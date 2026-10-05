# Portfolio Site Plan

## Goal
Create a publish-ready, root-level Jekyll site for Karim Osman at `karimosman1.github.io`, published from the `main` branch and repository root.

## Main-page content
- **Home:** introduction and selected experience.
- **About:** MBA and engineering education, technical skills, languages, volunteering, clubs, and interests.
- **Work Experience:** supplied roles and achievements at ETHOS AI, Oliver Wyman, and Booz Allen Hamilton.
- **Contact:** confirmed LinkedIn profile, email address, and phone number; no contact form.

The homepage combines these sections into one page with native, collapsible disclosures and top-right anchor navigation. The previous About, Work Experience, and Contact URLs redirect to the corresponding homepage sections. All biography and achievement details come from the supplied résumé or later user-confirmed updates.

## Design and implementation
- Light-only, responsive, accessible, single-column layout with a technical typographic feel; no reference sites were provided.
- Semantic HTML, native `<details>`/`<summary>` sections, plain CSS, reusable Jekyll layouts/includes, and Markdown with YAML front matter; no JavaScript is needed.
- Root-level `_config.yml`, `index.md`, `_layouts/`, `_includes/`, assets, SEO metadata, sitemap, favicon, and README.
- No backend, database, blog, CMS, form backend, framework, unnecessary libraries, or third-party trackers.

## Assumptions and verification
- GitHub username is `karimosman1`, confirmed from the connected GitHub account.
- The site will use an original, restrained visual treatment because no reference websites were supplied.
- Verify root-level GitHub Pages structure, navigation, responsive layout at 375px and 1280px, and Lighthouse targets of 90+ in Performance, Accessibility, Best Practices, and SEO.
- Explain technical choices and keep assumptions listed separately in the README.