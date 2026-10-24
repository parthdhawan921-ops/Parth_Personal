# Parth Dhawan · Data Analyst portfolio

An interactive résumé website. One file (`index.html`) plus a photo, with no build step and no frameworks.

**How it works**
- A recruiter picks the role they are hiring for: **Data / BI**, **Business / Ops**, **Product / Growth** or **Finance / Research**.
- The page rebuilds around that role: the headline, the "findings ledger" receipt, the order of the four featured projects, the skills table and the resume view.
- Each role has its own link, so every resume can point straight to its matching version of the site:
  - `…/#data` · `…/#business` · `…/#product` · `…/#finance`
- Each project also has its own link that opens its case file directly, e.g. `…/#cart` or `…/#sqlwh`.

**What's on it**
- 8 projects, each with question → answer → headline numbers → a live model you can play with → what I caught → method → limits → GitHub link
- "Mistakes I caught before they reached a report": real data problems found and fixed across the projects
- A skills table that links every skill to the project that proves it
- A role-tailored, one-page resume view (Save as PDF on the live site)
- About (pharmacy to analytics), certificates, and contact details with one-click copy
- Light and dark themes, a quick menu (Ctrl K / ⌘K), and keyboard shortcuts 1–4 to switch roles

Every number comes from the project repos. The live models are simplified rebuilds of each project's own calculations and reproduce its published figures.

## Preview on your computer
Run `python -m http.server` in this folder and open http://localhost:8000.

## Put it online (free)
**GitHub Pages**
1. Repo → **Settings → Pages**.
2. Source: **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
3. After a minute the site is live at `https://parthdhawan921-ops.github.io/Parth_Personal/`.

## Edit the content
All content lives in the `<script>` at the bottom of `index.html`:
- `P`: the 8 projects (text, numbers, GitHub repo, method, limits, resume bullets)
- `R`: the 4 roles (headline, receipt lines, which projects are featured and in what order)
- `CV`: resume title, summary and skills per role
- `SK`: the skills table · `CATCH`: the "mistakes I caught" cards

To make a private project's link appear, set its `repo` to the repository name (for example, `repo:'email-uplift-targeting'`).
