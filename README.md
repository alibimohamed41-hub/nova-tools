# NovaTools

A responsive, bilingual (French and Arabic) tools website built with plain HTML, CSS, and JavaScript. Designed for easy publishing on GitHub Pages.

## Features

- Responsive layout for phones, tablets, and desktop
- French and Arabic interface with RTL layout for Arabic
- Animated cards and hero illustration
- Quick Notes saved in the current browser
- Password generator using the browser's cryptographic random generator
- Word, character, and line counter
- Unit converter for length, weight, and temperature
- Focus timer
- QR-code creation using a third-party QR service
- Demo login/profile stored locally in the browser (not a secure authentication system)
- Search/filter tools

## Files

- `index.html` — page structure
- `style.css` — design and responsive styles
- `script.js` — tool behavior and language translations

## Run locally

Open `index.html` in a modern browser. The QR tool needs an internet connection because it calls an external QR service. Google Fonts are also loaded externally; the site falls back to system fonts.

## Publish on GitHub Pages

1. Sign in to GitHub and create a new repository, for example `novatools`.
2. Upload `index.html`, `style.css`, `script.js`, and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch `main` and folder `/ (root)`, then click **Save**.
6. Wait for GitHub to finish deploying. The Pages URL will appear in that section.

## Important notes

- The login is a front-end demo only. It stores a display name in `localStorage`; it does not verify identities, store passwords, or provide real account security.
- Notes are stored in the current browser using `localStorage`. Clearing browser data may delete them.
- QR code generation sends the entered text/link to `api.qrserver.com`. Do not use it for private or sensitive content.
- No build step or framework is required.
