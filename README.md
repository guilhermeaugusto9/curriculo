# Guilherme Augusto — Static Portfolio Refactor

A redesigned, bilingual (English-first / Portuguese) professional portfolio built with plain HTML, CSS and JavaScript. It is designed for GitHub Pages and requires no build step, server, database, package installation or API key.

## Preview locally

Open `index.html` in a browser. For a local HTTP preview, run `python3 -m http.server 8000` from this directory and visit `http://localhost:8000`.

## Publish to GitHub Pages

1. Review all professional statements, dates, project links and the downloadable résumé.
2. Copy the contents of this directory into the repository root used by GitHub Pages (or replace the existing site files in a branch first).
3. Commit and push to the branch/folder configured in **Settings → Pages**.
4. Verify the deployed site, language switch, mobile navigation, résumé PDF and every external link.

## Design and implementation decisions

- **English-first:** English is the default for new visitors; the language switch changes the content to Portuguese. The visitor's choice is stored locally when browser storage is available.
- **Static by design:** all content is in HTML and JavaScript. No server-side logic or runtime API is required. Google Fonts is an optional external font enhancement; the page has local system fallbacks if unavailable.
- **Communication, not inflated claims:** copy emphasizes scope, domain and responsibilities while avoiding invented impact metrics. Private company work is explicitly labelled as internal.
- **Skills by domain:** no percentage/proficiency bars; technologies are grouped by how they are used.
- **Accessible interaction:** semantic landmarks, skip link, visible focus defaults, language control labels, responsive mobile navigation and reduced-motion support.
- **SEO and sharing:** title, description, canonical URL, Open Graph, Twitter card and Person structured data.
- **Performance:** no framework or icon library required; profile image is local and prioritized; project content is rendered from compact local data.
- **Print:** CSS print styles provide a simplified printable version. The supplied PDF is included as a separate résumé download.

## Project structure

- `index.html` — semantic page structure, metadata and JSON-LD.
- `styles.css` — design system, layout, responsive styles and print rules.
- `app.js` — English and Portuguese copy and client-side rendering.
- `assets/profile.jpeg` — profile image supplied for this refactor.
- `assets/guilherme-augusto-cv.pdf` — résumé PDF supplied for this refactor.

## Before publishing

- Confirm that all wording accurately reflects your experience and that internal-company details are appropriate for public disclosure.
- Confirm the exact education wording for University of Washington / Coursera and any other credential that may need a more precise formal name.
- Check that the profile image is the intended public portrait and that you want the PDF available for download.
- Consider replacing the generic GitHub notebooks card with direct links to specific repositories/notebooks that you want recruiters to see.
- Confirm the canonical URL if the repository or Pages path changes.
- Consider adding a custom social preview image (1200×630) and a `404.html` if the site structure grows.

## Technical note

This is a no-build static site. It does not use npm at runtime. It deliberately does not introduce analytics trackers, contact forms requiring a backend, external content APIs or a CMS.
