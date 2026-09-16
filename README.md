# JCx3 — Cargill Family Sites

Static site for GitHub Pages. `index.html` is the master index: every page in the repo, what it's for, who uses it, and when to open it.

| File | Page |
|---|---|
| `index.html` | Cargill Family Sites — master index (start here) |
| `board.html` | Cargill Family Board — progress, script, LLC, truck, benefits, links (views by hash: `#board #script #llc #truck #benefits #links`) |
| `plan.html` | Settlement Allocation Plan |
| `cargill-budget-site/index.html` | Cargill Household Budget — payday deposits, personal bills, 401(k), Q1 bonus, reimbursements, checklist |
| `cargill-budget-site/llc.html` | Cargill Consulting Ledger |
| `cargill-llc-ledger/index.html` | Consulting Ledger, stand-alone copy for sharing on its own |

## Publish
Upload everything to the root of `main`. Settings → Pages → Deploy from a branch → `main` / `/ (root)`. The site appears at `https://<username>.github.io/JCx3/`.

## Editing
Budget and ledger pages save edits in each viewer's own browser (localStorage). To change the shared plan, edit the `D = {...}` defaults in the page script and re-upload.

`noindex` is set on every page, but a public repo is public to anyone with the link — these pages hold household financial figures.
