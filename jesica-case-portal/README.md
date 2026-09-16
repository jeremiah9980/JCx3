# Jesica's Case Portal

A single-page, plain-English reading guide to *In re Jesica Ann Green*, Chapter 13, Case No. 26-80641 (Bankr. S.D. Tex., Galveston). No build step, no dependencies — `index.html` plus the court's own PDFs in `docs/`.

## Publish on GitHub Pages

1. Create a repository (see the privacy note below before choosing public or private).
2. Upload everything in this folder to the repository root — `index.html`, `README.md`, `robots.txt`, `.nojekyll`, and the `docs/` folder.
3. Repository **Settings → Pages → Source: Deploy from a branch → Branch: main / (root)** → Save.
4. The site appears at `https://<username>.github.io/<repo>/` within a minute or two.

`.nojekyll` stops GitHub from running Jekyll, so the `docs/` folder and its filenames are served exactly as-is.

## Privacy — read this first

The PDFs are public court records, but they still contain the last four digits of a Social Security number (Doc 12, Claim 2-1, docket sheet), a personal phone number and email address (Doc 6), and a home address throughout.

- **GitHub Pages sites are always public**, even from a private repository. Anyone with the URL can open every PDF. `robots.txt` and the `noindex` tag discourage search engines but do not block a visitor.
- If that's not acceptable, keep the repository **private and don't enable Pages** — Jesica can download the repo (or this zip) and open `index.html` straight from her computer; everything works offline.
- Middle ground: publish, but strip Doc 6's phone/email by re-downloading a redacted copy, and share the URL only with her.

## Adding a new document

1. Save the PDF from PACER into `docs/` using the same naming pattern: `doc-NN_YYYY-MM-DD_short-title.pdf` (or `claim-N-N_...`).
2. In `index.html`, add an object to the `DOCS` array (id, docket number, date, who filed it, title, file path, page count, and a one-paragraph plain-English summary).
3. Add a matching entry to `TIMELINE`, and to `DATES` if the paper sets or changes a deadline.
4. Update the "Docket last pulled" line in the header and, when an order dismissing the case is entered, rewrite the banner in the **Where things stand** section.

## What's not included

Docket entries 1 (petition), 3 (Statement of SSN — sealed), 4 (Pro Se Filer Identification) and 7 (fee receipt) were not downloaded. Claim 1-1 has not been pulled. The Louisiana case that shares the number 26-80641 (a different debtor, Western District of Louisiana) is deliberately excluded.

Nothing here is legal advice.
