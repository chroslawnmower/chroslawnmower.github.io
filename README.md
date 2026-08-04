# chroslawnmower.github.io

Personal academic site for Christopher Lohmeyer. Plain static HTML, no build step.

## Files

- `index.html` — the entire page (inline styles, two Google Fonts, no framework)
- `photo.jpg` — profile photo shown in the about section
- `cv.pdf` — linked from the nav and from the "Download CV (PDF)" button
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Publishing to GitHub Pages

1. Create a repo named `chroslawnmower.github.io` (user site, served at the root domain).
2. Copy the contents of this folder into the repo root and push to `main`.
3. In the repo, go to Settings → Pages, set Source to "Deploy from a branch", branch `main`, folder `/ (root)`.
4. The site appears at https://chroslawnmower.github.io within a minute or two.

For a project repo instead (e.g. `portfolio`), the same steps apply and the URL becomes https://chroslawnmower.github.io/portfolio/.

## Updating content

Everything is in `index.html`. Sections are marked with `id` attributes matching the nav links: `#about`, `#research`, `#publications`, `#news`, `#work`, `#education`.

To replace the CV, overwrite `cv.pdf` and keep the filename. To replace the photo, overwrite `photo.jpg`.

## Known TODOs

- MABEL and the AIAA SciTech paper are not yet cleared for public release; the descriptions on the page are deliberately kept to a high level. Add a repo link and a DOI once both are approved.
- No LinkedIn button yet. To add one, copy the GitHub anchor in the footer row and change its `href` and label.
- Responsive rules live in the `@media (max-width: 760px)` block in `<head>`.
