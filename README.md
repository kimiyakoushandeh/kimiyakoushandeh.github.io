# Kimiya Koushandeh — Resume / Portfolio Site

Custom static single-page resume site for **Kimiya Koushandeh (Product Designer)**, built for GitHub Pages.

- **Live site (after publish):** https://kimiyakoushandeh.github.io/
- **Stack:** hand-written HTML, CSS, and a small amount of vanilla JS (no build step)

## Structure

```text
.
├── index.html                  # Main single-page site
├── styles.css                  # Design tokens, layout, components, responsive/print styles
├── script.js                   # Mobile nav, smooth scroll, scroll reveals (reduced-motion aware)
├── assets/
│   ├── resume.pdf              # Downloadable CV (replace with final PDF)
│   ├── favicon.svg             # Site icon
│   ├── og-image.png            # TODO: add 1200x630 social preview image
│   └── work/
│       └── credit-flow/        # TODO: add 1–3 project screenshots/mockups
├── case-studies/
│   └── credit-flow.html        # Placeholder case study page (ready to expand later)
├── .nojekyll                   # Disable Jekyll processing on GitHub Pages
└── README.md
```

## Local preview

Open `index.html` directly in a browser for a quick check, or run a local server from the repo root for the most accurate behavior:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy (GitHub Pages user site)

This repo is intended to be the user site repo: `kimiyakoushandeh/kimiyakoushandeh.github.io`.

1. Push changes to the default branch (`main`).
2. In GitHub: **Settings → Pages**.
3. Set **Source** to *Deploy from a branch*.
4. Select branch `main` and folder `/ (root)` and save.
5. The site will be published at https://kimiyakoushandeh.github.io/

## Before publishing (TODO checklist)

- [ ] **Verify content:** confirm dates, titles, and wording (especially role date ranges and course labels) against the final resume.
- [ ] **Links:** add verified LinkedIn/portfolio/Behance/Dribbble URLs and the exact Credit Application Flow Redesign/case-study URL (remove `TODO` link placeholders).
- [ ] **Contact privacy:** confirm what to show publicly (default: email only). Add phone/location details only if explicitly approved.
- [ ] **Resume PDF:** replace `assets/resume.pdf` with the final, approved PDF.
- [ ] **Project visuals:** add 1–3 screenshots/mockups to `assets/work/credit-flow/` and wire them into the featured work card / case study.
- [ ] **Case study:** expand `case-studies/credit-flow.html` with real narrative, visuals, and outcomes when available.
- [ ] **Social preview:** add `assets/og-image.png` (1200×630) and confirm meta tags/URL.
- [ ] **QA:** test on mobile and desktop, check keyboard navigation/focus states, contrast, print view, and that all links/assets work.

## Notes

- Content is kept faithful to the provided resume; placeholder/TODO markers are used where links, visuals, or confirmations are still needed.
- Motion/animations respect `prefers-reduced-motion`.
- A print stylesheet is included so the page prints cleanly alongside the downloadable CV.
