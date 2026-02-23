# Farid Salazar Academic Website

Clean, minimalist, single-page academic site built with plain HTML/CSS for easy GitHub Pages deployment.

## Directory Structure

```text
.
├── CNAME.example
├── README.md
├── index.html
└── assets
    ├── css
    │   └── styles.css
    ├── files
    │   └── Farid_Salazar_CV.pdf
    └── img
        └── portrait-placeholder.svg
```

## Deploy on GitHub Pages

1. Create a GitHub repository (for user site, use `<username>.github.io`).
2. Push these files to the default branch (`main`).
3. In GitHub: **Settings > Pages**.
4. Under **Build and deployment**, choose:
   - Source: **Deploy from a branch**
   - Branch: `main` and folder `/ (root)`
5. Save and wait for deployment.

Your site will be available at:
- `https://<username>.github.io/` (or your repository Pages URL)

## Custom Domain Setup (CNAME)

1. Rename `CNAME.example` to `CNAME`.
2. Edit its single line to your real domain (for example `faridsalazar.com`).
3. Configure DNS at your registrar:
   - Apex domain (`faridsalazar.com`): A records to GitHub Pages IP addresses
   - `www` subdomain: CNAME to `<username>.github.io`
4. In GitHub Pages settings, ensure custom domain is detected and enable HTTPS.

## Customize Content

- Main content: edit `index.html`
- Site styles: edit `assets/css/styles.css`
- Portrait image: replace `assets/img/portrait-placeholder.svg` and update `src` in `index.html` if needed
- CV file: replace `assets/files/Farid_Salazar_CV.pdf` with your real CV PDF
- Contact details and links: edit the `#contact` and `#publications` sections in `index.html`

## Add New Pages Later

1. Create a new HTML file in the root (example: `research.html`).
2. Reuse the same stylesheet by adding:

```html
<link rel="stylesheet" href="assets/css/styles.css" />
```

3. Add a navigation link in `index.html`:

```html
<a href="research.html">Research</a>
```

4. Commit and push; GitHub Pages redeploys automatically.

## Notes

- No JavaScript framework required.
- Fully static and GitHub Pages compatible.
- Responsive and keyboard-accessible with semantic HTML.
