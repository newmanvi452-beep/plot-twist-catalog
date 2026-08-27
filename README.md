# Plot Twist — catalogue

The book catalogue for the Plot Twist iOS app. This repository is public so
the app can fetch it directly; the app's source is private.

`catalog.json` holds a `version` and a list of books. The app ships with a
copy bundled, fetches this one on launch, and only adopts it when `version`
is higher than the copy it already has. An unchanged file costs a 304 and no
body, so checking is close to free.

Books are added by the ingestion pipeline in the app repo, which sources real
ISBNs from Open Library and hand-labels each book against the same vocabulary
the onboarding questions use.

## Publishing

Two things to know, both learned the hard way:

**Publish here as well as to the app repo.** The catalogue lives in both:
`PlotTwist/Data/catalog.json` is bundled into the build, and this copy is what
installed apps fetch. Updating only the app repo means existing readers never
see the new books, and the app ignores this copy silently because it compares
versions before adopting — an older copy here simply loses.

**raw.githubusercontent.com caches for five minutes.** `cache-control:
max-age=300`, so a push is not immediately visible at the raw URL. Check the
`source-age` response header before concluding the push failed; the API
(`gh api repos/.../contents/catalog.json`) shows the truth straight away.

Raw URL the app reads:

    https://raw.githubusercontent.com/newmanvi452-beep/plot-twist-catalog/main/catalog.json
