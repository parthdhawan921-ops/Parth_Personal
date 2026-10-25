# Parth Dhawan · Data Analyst portfolio

An interactive résumé website. One file (`index.html`) plus a photo, with no build step and no frameworks.

**How it works**
- A recruiter picks the role they are hiring for: **Data / BI**, **Business / Ops**, **Product / Growth** or **Finance / Research**.
- The page rebuilds around that role: the headline, the "findings ledger" receipt, the featured projects and their order, the skills list and the resume.
- Each role has its own link, so every resume can point straight to its matching version of the site:
  - `…/#data` · `…/#business` · `…/#product` · `…/#finance`
- Each project also has its own link that opens its case file directly, e.g. `…/#cart` or `…/#sqlwh`.

**What's on it**
- 11 projects, each with question → what I did → what I found → why it matters → a live model you can play with → method → limits → GitHub link (and slides for 4 of them)
- "Mistakes I caught before they reached a report": real data problems found and fixed across the projects
- A skills list that links every skill to the projects that prove it
- The one-page PDF resume for each role, shown on the page with Open and Download buttons (`assets/resume/`)
- Real screenshots from each project (dashboards, notebook and Excel charts, a SQL query and its result) in `assets/shots/`
- A link-preview card (`assets/og.jpg`) so the link shows your photo and headline on LinkedIn and WhatsApp
- About, certificates, and contact details with one-click copy
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
- `P`: the 11 projects (text, numbers, GitHub repo, slides, method, limits)
- `R`: the 4 roles (headline, receipt lines, which projects are featured and in what order)
- `PDF`: the resume file for each role (PDFs and page previews in `assets/resume/`)
- `SK`: the skills list · `CATCH`: the "mistakes I caught" cards

To make a private project's link appear, set its `repo` to the repository name (for example, `repo:'email-uplift-targeting'`).

The resume PDFs are printed from the resume view. After changing `P` or `CV`, open the resume view in Chrome, pick the role, press Ctrl+P and save as PDF to `assets/resume/` with the same file name.
