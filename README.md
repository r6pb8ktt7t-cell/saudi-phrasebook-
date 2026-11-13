# Saudi Phrasebook — early working build

A multilingual phrasebook prototype for Uzbek, Russian and English speakers travelling in Saudi Arabia.

## Included
- Fusha and general Saudi colloquial variants for each phrase
- Uzbek, Russian and English interface translations
- Category filtering, text search and local favorites
- Responsive layout and installable PWA manifest
- Service-worker app-shell caching for repeat offline visits
- Optional device speech synthesis for Arabic pronunciation

## Run / publish
Serve this folder over HTTPS (or localhost for development). For GitHub Pages, publish the repository root from the `main` branch in repository Settings → Pages. Open the published HTTPS address once while online; the service worker then caches the app shell.

## Important limitations — not release-ready
- The current phrase set is a starter set, not a professionally reviewed phrasebook. Saudi colloquial speech varies by region; a native Saudi Arabic reviewer must verify every phrase, transliteration and usage note before public release.
- The play button uses the browser/device speech synthesis engine when an Arabic voice is installed. These are not human studio recordings and availability/quality varies by device. The generated speech is not guaranteed to work offline.
- The service worker caches the app interface and phrase data after the first successful online visit. Offline behavior still needs real-device testing (iOS Safari, Android Chrome, and desktop).
- This build does not yet contain recorded audio files, full phrase coverage, regional labels, automated tests, or native App Store / Play Store packages.

## Privacy
Favorites are stored locally in the browser using localStorage. No account or server is used by this app.
