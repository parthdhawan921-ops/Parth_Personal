# Parth Dhawan · Data Analyst portfolio

An interactive résumé website. One file (`index.html`), no build step, no frameworks.

**What's on it**
- A "findings ledger" receipt in the hero with the headline result of each project
- Four case files (cart leakage, email uplift, dark-store break-even, retail pipeline), each with
  question → answer → a live model you can play with → method → limits → links
- A skills matrix that links every skill to the project that proves it
- Journey and certificates, contact with one-click email copy
- Light / dark theme, and a quick menu (Ctrl K / ⌘K)

Every number comes from the project repos. The live models are simplified rebuilds of each
project's own calculations and reproduce its published figures.

## Preview on your computer
Double-click `index.html`, or run `python -m http.server` in this folder and open http://localhost:8000.

## Put it online (free)
**Option A: Vercel (works with a private repo)**
1. Go to https://vercel.com and sign in with GitHub.
2. Click **Add New → Project**, pick `Parth_Personal`, choose the branch with `index.html`.
3. Framework preset: **Other**. Leave build settings empty. Click **Deploy**.
4. You get a link like `parth-dhawan.vercel.app`. Rename it in Settings → Domains.

**Option B: GitHub Pages (repo must be public on a free plan)**
1. Repo → **Settings → Pages**.
2. Source: **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
3. After a minute the site is live at `https://parthdhawan921-ops.github.io/Parth_Personal/`.

## Edit the content
All text is plain HTML in `index.html`. Project numbers for the live models are at the top of
each block in the `<script>` at the bottom (search for `A1`, `A2`, `A4`, `Pipeline`).
