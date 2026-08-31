# Privacy Policy for Plot Twist

**Last updated: August 30, 2026**

Plot Twist is a book recommendation app. This page explains what the app does and doesn't do with your information.

## Your account

Plot Twist asks you to sign in with Apple so your shelf survives a reinstall or a new phone. We never see your Apple ID, your email, or a password — Apple handles that handshake and only ever gives us a random ID for your account and, the first time only, the name you've told Apple to share (if any).

Signing in syncs the following to your account, so it can come back down to any device you sign into:

- Your taste answers from onboarding (genres, pace, romance level, spice comfort, dealbreakers)
- Your shelves (to-read, currently reading, read, passed)
- Ratings, tags, and notes you add when you finish a book
- Your display name, birthday, and profile photo, if you choose to add them

This data is yours, tied to your account, and not shared with or sold to anyone else — no advertising, no data brokers, nothing correlated across other apps or companies. It's stored with Supabase, our database provider, acting only as infrastructure on our behalf.

You can delete your account from inside the app at any time (Edit Profile → Delete Account). This permanently removes your account and everything synced to it — there's no recovery after that point.

Your birthday, if you add one, is used only to set an age-appropriate ceiling on how explicit a book's content rating can be, and to notice your birthday week for a small in-app touch.

Theme and a couple of small session preferences stay local to your device and aren't synced.

## The one thing we collect that isn't tied to your account

When you add a book to your shelf that isn't yet in Plot Twist's catalogue, the app tells us that book's title, author, and ISBN, and how many readers have asked for it. That's it — no account ID, no device ID, no name, no rating, no shelf, no timestamp, and nothing that can be linked back to you or your device. We use this only to decide which books to add to the catalogue next. It can't be connected to any other report, and it can't be traced to a person.

## Requests that leave your device

A few things Plot Twist does require talking to the internet:

- **Signing in and syncing.** Signing in and keeping your shelf in sync talks to Apple (to verify who you are) and to our database provider, Supabase (to store and retrieve your account data described above).
- **Fetching the book catalogue.** The app periodically checks for an updated list of books. This is a simple request for a public file — nothing about you is sent with it.
- **Searching for a book.** If you search for a book to add to your shelf, your search text is sent to [Open Library](https://openlibrary.org), a free and open book database run by the nonprofit Internet Archive, so we can show you results. We don't attach anything else to that request.
- **Book cover art.** Cover images are fetched from Open Library's cover service using the book's ISBN — no reader data involved.
- **"Get it" links.** If you tap a link to buy or borrow a book, Plot Twist opens that retailer's website (for example, Bookshop.org) in your device's browser. Once you leave the app, that site's own privacy policy applies — we don't receive any information back about what you did there, including whether you bought anything.

## Analytics

Plot Twist does not currently send app usage data to any analytics service. If that changes in the future, we'll update this policy first.

## Children's privacy

Plot Twist is not directed at children under 13, and we don't knowingly collect information from children. The age-based content filter described above is calculated and enforced entirely on your device from a birthday you optionally provide — the filtering decision itself never leaves your phone, even though the birthday value syncs with the rest of your account data if you're signed in.

## Changes to this policy

If anything here changes, we'll update this page and change the date at the top.

## Contact

Questions about this policy? Reach out at sundaylogicapps@gmail.com.
