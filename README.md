# Character Rise - Privacy Policy site

Public GitHub Pages site that hosts the Character Rise privacy policy.

**Purpose:** The main `Character-Rise` repo must stay **private** (it contains the
app source and references to the signing config). Publishing the policy from a
**separate public repo** keeps the code private while giving Google Play a
publicly-accessible privacy URL.

**URL after deployment:** `https://shakeyourmoneymaker.github.io/Character-Rise-Privacy-Policy/`
(the site name follows `<username>.github.io/<repo>/`).

## Deploy

1. Create the **Public** repo `Character-Rise-Privacy-Policy` on GitHub
   (New repository -> name `Character-Rise-Privacy-Policy`, **Public**, no README).
2. Push from this folder:
   ```powershell
   cd C:\Users\Charles\Documents\Default Project\Character-Rise-Privacy-Policy
   git push -u origin main
   ```
   (local repo is already initialized and committed; the first push may ask
   you to sign in to GitHub in a browser window.)
3. Repo settings -> Pages -> Source: **Deploy from a branch**, branch `main` / root -> Save.
4. Your URL is live (allow ~1 min): `https://shakeyourmoneymaker.github.io/Character-Rise-Privacy-Policy/`
5. Paste that URL into the Play listing **Privacy policy URL** field and into
   `play-store-listing/store-listing.md`.

## Housekeeping
- Update `index.html` any time the policy changes (rename it — the file to edit
  is `index.html`, the policy lives in the app docs folder as
  `play-store-listing/privacy-policy.html`; keep them in sync).
- Do NOT put the app source or secrets in this public repo.