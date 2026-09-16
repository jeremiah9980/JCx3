# Cargill Household Budget

Static pages, no build step, no server. Upload to GitHub Pages (or any static host) and share the URL.

- `index.html` — household budget portal: payday deposits by account, personal bills (Jeremiah / Jesica / Cooper), 401(k), Q1 bonus, medical reimbursements, and the couple's checklist (payday / monthly / quarterly / annual).
- `llc.html` — Cargill Consulting LLC ledger: funding in, spend with tax value, truck depreciation, expected project revenue, and the commitment gate.

## Publish on GitHub Pages
1. Create a repo (on a free plan it must be public for Pages; private works on paid plans).
2. Upload the files to the repo root.
3. Settings -> Pages -> Source: Deploy from a branch -> main / root -> Save.
4. The site appears at https://<user>.github.io/<repo>/ within a minute or two.

## How editing works
Every dashed number is editable and every total recalculates. Edits, "paid" ticks and checklist ticks are saved in the viewer's own browser (localStorage), so each person sees their own — run the payday checklist together on one device. To change the shared plan itself, edit the `D = {...}` and `CK = {...}` defaults blocks in the page's script and re-upload; "Reset to plan" on the page returns a viewer to those defaults.
