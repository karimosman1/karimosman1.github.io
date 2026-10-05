# Karim Osman — personal portfolio

A static Jekyll site for `karimosman1.github.io`. The site source is in this repository’s root so GitHub Pages can publish it directly from the `main` branch and `/(root)`.

## Publish with GitHub Pages

1. Create or use the GitHub repository named `karimosman1.github.io`.
2. Put these root-level files on the `main` branch.
3. In the repository’s **Settings → Pages**, choose **Deploy from a branch**, select `main`, and select `/(root)`.
4. Save. GitHub Pages builds the Jekyll site itself; no separate build workflow or generated `dist` folder is needed.

The configured site URL is `https://karimosman1.github.io` and `baseurl` is intentionally empty for a GitHub user site.

## Update the content

- Edit `index.md`, `about.md`, `work-experience.md`, or `contact.md`. Each page uses YAML front matter for its title, description, and URL.
- Shared navigation is in `_config.yml`; the common page layout and reusable header, footer, and head elements are in `_layouts/` and `_includes/`.
- Update styling in `assets/css/styles.css` and the browser icon in `assets/images/favicon.svg`.
- The Contact page publishes Karim's confirmed LinkedIn profile and a tap-to-call phone link. Update those details in `contact.md`.
- No public email address, contact form, or JavaScript is included.

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
- The pages use semantic HTML, a shared accessible layout, and local system fonts; no third-party trackers or client-side libraries are loaded.

## Assumptions

- No reference websites were provided, so the visual treatment is original, light, and technical.
- The LinkedIn profile URL and phone number are confirmed for public display on the Contact page; the email address remains unpublished.
- Résumé facts are used as provided; no employers, clients, achievements, or metrics have been added.