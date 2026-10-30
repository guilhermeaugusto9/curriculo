# Refactor notes

## Direction
- Shifted the brand voice from informal slogans to a professional value proposition: “Turning data into business value.”
- Made English the default and added a Portuguese language switch.
- Replaced the legacy Bootstrap/Font Awesome/Gulp-style setup with a lightweight native HTML/CSS/JavaScript implementation.
- Introduced a new visual system: dark editorial layout, restrained lime accent, typography hierarchy, generous spacing, structured timeline and domain-based skill cards.

## Content architecture
- Reframed the profile around Data & Analytics Engineering, BI, Data Strategy and applied AI.
- Grouped technologies by domain rather than a flat list.
- Removed subjective proficiency percentages/bars.
- Kept career details anchored in the provided portfolio and résumé; company-internal AI work is labelled as internal.
- Included selected public links and marked private work accordingly.

## Technical improvements
- Responsive layouts and mobile navigation.
- Keyboard skip link and semantic page landmarks.
- Reduced-motion support and print styles.
- SEO metadata, canonical URL, Open Graph/Twitter metadata and Person JSON-LD.
- No build step, server, API key or runtime dependency.

## Caveats / next iteration
- Review all dates and credential phrasing before publishing.
- The source material has overlapping concurrent roles (e.g. teaching and freelance work); dates are preserved rather than normalized.
- Project links are drawn from the existing portfolio; validate each destination and replace generic GitHub links with selected repositories when possible.
- Search ranking is not guaranteed by metadata; the content's clarity, crawlability and relevant external profiles matter more than keyword stuffing.
