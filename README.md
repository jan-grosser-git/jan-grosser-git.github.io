This repository is used for my website - for now as an experiment.

Wesbite is found under: https://jan-grosser-git.github.io/

## Structure

Single static `index.html` (HTML + inline CSS/JS), hosted on GitHub Pages. No build step.
Sections are signposted with `<!-- ════ SECTION: … ════ -->` comments; styling lives in the
matching `/* ── … ── */` block inside `<style>`.

## Writing section — future option

The Writing section is currently authored **inline** in `index.html`: each piece is an
`<article class="writing-item">` block you copy and edit by hand. This is fine for a handful
of short notes.

If it grows (roughly 5+ posts, or a need for per-post URLs and dates), migrate to **Jekyll**,
which GitHub Pages runs natively — no backend or external service required:

- Write each post as a Markdown file in a `_posts/` folder (`YYYY-MM-DD-title.md`).
- Add a `_config.yml` and a layout; Jekyll builds the posts into pages automatically.
- Gains: individual shareable URLs, automatic dated index, Markdown authoring instead of HTML.
- Cost: introduces a build step and project structure (layouts/config), so it's a step up from
  the current single-file setup.

Until then, the inline approach stays static and matches the existing design system.
