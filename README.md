# Calhoun County FRN — Wraparound Services Directory

A responsive, accessible, no-build static website for GitHub Pages. Uses plain HTML/CSS/JavaScript and `providers.json`. No tracking, accounts, or client data storage.

## Deploy to GitHub Pages
1. Create a public GitHub repository (suggested: `calhoun-frn-resources`).
2. Upload **all four files** (`index.html`, `styles.css`, `app.js`, `providers.json`) to the repository root. (README is optional.)
3. Go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, select `main` and `/(root)`, then **Save**.
4. Open the GitHub Pages URL once the deployment completes.

## Maintain the directory
- Edit `providers.json` directly in GitHub to add or update records. Follow the existing object format and give every provider a unique `id`.
- Keep `category` as an array of existing or new category labels; the website generates filters automatically.
- Use `scope`: `Local`, `Regional`, `Statewide`, or `Nationwide`.
- Set `checked` to the date you actually checked the official source. Never change dates automatically.
- Add a public `source` URL and verify that services really cover Calhoun County.
- Confirm phones, eligibility, hours and referral steps by phone before distributing widely.

## Important limitations
- This is a **public resource listing**, not a referral management system or secure intake form. Do not add names, case notes, medical details or other client information to JSON, GitHub issues or public repository files.
- Online source verification was completed November 5, 2026 for the initial listings. Live phone confirmation and FRN editorial approval are still needed.
- No FRN logo was used because brand asset permissions have not been confirmed.
- Open `index.html` through GitHub Pages or a local web server (e.g. `python -m http.server`); opening as a local `file://` URL can prevent JSON loading.


## Red theme update (November 2026)
This version updates `styles.css` and the browser theme color in `index.html` to a coordinated burgundy/crimson/blush palette. Directory data and behavior are unchanged. To update an existing GitHub Pages site, replace **only** `styles.css` and `index.html` in the repository root, then commit.
