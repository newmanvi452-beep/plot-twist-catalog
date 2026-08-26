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

Raw URL the app reads:

    https://raw.githubusercontent.com/newmanvi452-beep/plot-twist-catalog/main/catalog.json
