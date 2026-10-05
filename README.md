# Karim Osman — personal portfolio

A static, single-page Jekyll portfolio for `karimosman1.github.io`. The site source is in this repository’s root so GitHub Pages can publish it directly from the `main` branch and `/(root)`.

## Publish with GitHub Pages

1. Create or use the GitHub repository named `karimosman1.github.io`.
2. Put these root-level files on the `main` branch.
3. In the repository’s **Settings → Pages**, choose **Deploy from a branch**, select `main`, and select `/(root)`.
4. Save. GitHub Pages builds the Jekyll site itself; no separate build workflow or generated `dist` folder is needed.

The configured site URL is `https://karimosman1.github.io` and `baseurl` is intentionally empty for a GitHub user site.

## Update the content

- Edit `index.md` to update the homepage, résumé sections, and contact details.
- The top-right navigation in `_config.yml` jumps to sections on the homepage. The old `/about/`, `/work-experience/`, and `/contact/` URLs redirect to those sections.
- The common page layout and reusable header, footer, and head elements are in `_layouts/` and `_includes/`.
- Update styling in `assets/css/styles.css` and the browser icon in `assets/images/favicon.svg`.
- The Contact page publishes Karim's confirmed LinkedIn profile, email link, and tap-to-call phone link. Update those details in `contact.md`.
- The collapsible sections use native HTML; no JavaScript, contact form, or client-side library is included.

## Preview locally

Ruby and Bundler are required. The `github-pages` gem in `Gemfile` provides the same Jekyll and plugin family used by GitHub Pages.

```sh
bundle install
bundle exec jekyll serve
```

Open the local address printed by Jekyll. Changes to Markdown, layouts, and CSS are served locally; GitHub Pages publishes from the repository root.

## Check with Lighthouse

With the local Jekyll preview running, open the site in Chrome. In Chrome DevTools, open **Lighthouse**, select **Navigation**, and run the Performance, Accessibility, Best Practices, and SEO audits. Check the responsive layout at 375px and 1280px in the device toolbar.

## Technical choices

- GitHub Pages’ built-in Jekyll publishing keeps the site static and avoids a custom deployment workflow.
- `jekyll-seo-tag` supplies canonical and social metadata; `jekyll-sitemap` generates the sitemap.
- Internal navigation and asset paths use Jekyll’s `relative_url` filter, while the GitHub user-site `baseurl` remains empty.
- The page uses semantic HTML, native keyboard-accessible disclosure sections, and local system fonts; no third-party trackers or client-side libraries are loaded.

## Assumptions

- No reference websites were provided, so the visual treatment is original, light, and technical.
- The LinkedIn profile URL, email address, and phone number are confirmed for public display on the Contact page.
- Résumé facts are used as provided; no employers, clients, achievements, or metrics have been added.