# Privacy Policy

This web application collects nothing: no analytics, no telemetry, no tracking, no ads, no cookies and no third-party scripts. Nothing goes to the developer or to any server. The whole tool runs on your device.

## What is processed and where it stays

All of the following stays on your device and is never uploaded:

- The data points of the scooter, read over Bluetooth LE.
- The keys and settings you enter (localKey, srand, the dpId schema). The localKey and schema are stored locally in the browser (localStorage) only; srand is kept in memory for the session.
- Any Bluetooth capture you analyze. It is read and parsed entirely in the page and never leaves the device.
- The log on screen. It lives only in the open page. The device name and id, and the derived session key, are anonymized and credentials or tokens are redacted before anything is stored, shown, copied or saved.

## Network connections

- **Loading the page:** your browser fetches the static files from the host (for example GitHub Pages). The host sees your IP address and which file you requested, the usual access logs. Scooter data, keys or commands never reach any server.
- **Bluetooth LE to the scooter:** a local radio link, not an internet connection. Commands and the scooter replies run only between your browser and the scooter.
- **Nothing else.** The page's Content Security Policy allows `connect-src 'self'` only, so the page cannot talk to any other server even if it wanted to.

## Note on the official app

The official ISINWHEEL app is a Tuya "Smart Life" container that signs in to the Tuya cloud to resolve your product, its dpId schema and the per-device localKey. This page does **not**. It speaks only to the scooter over Bluetooth and needs no account; the localKey and srand you supply yourself.

## Contact

For privacy questions contact the author (Laufbursche) on GitHub: https://github.com/Laufbursche42
