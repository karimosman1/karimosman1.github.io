# Change 2: Single-page portfolio layout

## Goal

Improve the portfolio experience by bringing its information onto the main page and making key sections easy to reach.

## Requested changes

- Keep the introduction and selected experience at the top of the homepage.
- Consolidate the About, full Work Experience, and Contact content onto the homepage without losing résumé details or the confirmed contact links.
- Use native, accessible `<details>` and `<summary>` sections for About, Work Experience, and Contact. Start them open so visitors can see the information immediately, and let them collapse sections as needed.
- Change the top-right navigation from separate-page links to in-page jumps for Home, About, Work Experience, and Contact. Keep the navigation responsive on small screens.
- Preserve `/about/`, `/work-experience/`, and `/contact/` as redirects to the matching homepage sections, so existing links continue to work.
- Keep the site static and avoid adding JavaScript, a framework, or a backend.

## Branch

Apply the change on the current local `WebsiteLayout` branch. Do not push or merge it as part of this change.

## Acceptance criteria

- The homepage contains the existing introduction, education, skills, languages, volunteering, interests, complete work history, and contact details.
- Each top-right navigation link jumps to its corresponding homepage section.
- The sections can be expanded and collapsed using the keyboard or pointer.
- Existing section URLs lead to the corresponding content on the homepage.
- The Jekyll site builds, and this planning file is excluded from the published output.