# Copilot Instructions for elbow86.github.io

## Project overview

This repository is a personal blog and project portfolio built with Jekyll and hosted on GitHub Pages. The content is primarily Markdown pages and custom HTML/CSS embedded in the root-level pages; there is no application server, API layer, or unit-test suite to run beyond the Jekyll site build.

## Build, test, and validation commands

Use the repo's Bundler workflow from the project root:

```bash
bundle install
bundle exec jekyll build
bundle exec jekyll serve --livereload
```

Key notes:
- `bundle exec jekyll build` is the main validation step. It catches broken front matter, invalid Markdown, and broken Liquid/Jekyll rendering.
- `bundle exec jekyll serve --livereload` is the local preview workflow; open `http://127.0.0.1:4000`.
- If the generated site gets stale or a build appears stuck, run `bundle exec jekyll clean` before rebuilding.
- There are no dedicated JS/TS or Ruby test commands in this repo. Treat a successful Jekyll build as the default correctness check for content changes.

## High-level architecture

This is a static Jekyll site, not a traditional web app:

- `_config.yml` sets the site metadata, theme, and Jekyll options.
- `index.md` is the homepage and contains both front matter and custom HTML/CSS markup for the landing page and timeline cards.
- Blog entries are written as root-level Markdown files such as `2026-Jan-29.md`, `2026-Feb-1.md`, and `2026-May-24.md` instead of the usual `_posts/` structure.
- Jekyll renders these Markdown files to HTML at build time; links should therefore point to the generated HTML paths (for example `./2026-Jan-29.html`).
- `_site/` is generated output; do not edit it manually.
- `vendor/` contains the Ruby bundle used for local development.
- GitHub Pages deploys the site automatically from the default branch; there is no build pipeline logic in the repo itself beyond Jekyll.

## Project conventions that matter here

### Content layout and naming
- Blog posts live at the repository root, not under `_posts/`.
- Use date-based filenames such as `YYYY-MMM-DD.md` or monthly summaries like `YYYY-MMM.md`.
- Keep the title and filename aligned with the post date and subject.

### Front matter and page structure
Use the standard pattern for posts:

```yaml
---
layout: page
title: Your Post Title
---

# Your Post Title

Your content here...
```

- `layout: page` is the normal choice for standalone blog entries.
- `index.md` has a custom `layout: home` front matter and embeds the homepage cards and project sections directly in the page.

### Internal linking
- Prefer relative links to the generated HTML page: `[Link Text](./2026-Jan-29.html)`.
- Do not link to source Markdown files as if they were the published route; Jekyll publishes HTML.
- Use the same relative path convention for cross-post navigation and homepage cards.

### Homepage and changelog updates
When adding or changing posts, update the related content in the same repo:
- Add/update the relevant card or timeline item in `index.md`.
- Update `CHANGELOG.md` for user-visible content changes.
- Keep the post date in both the filename and the page content consistent.

### Styling conventions
- Styling is intentionally custom and inline-heavy rather than separated into a large stylesheet.
- The visual system uses the existing blue palette from the current homepage (`#1e3a5f`, `#2c5282`, `#4a6fa5`, and light card backgrounds).
- Reuse the same card patterns and subtle border accents instead of introducing a completely different layout style.

## Notes for future Copilot sessions

- Keep changes content-first: this repository is mostly static writing, reference links, and markdown pages.
- Prefer minimal edits that preserve the existing site tone and structure.
- Do not add framework or build tooling unless the project explicitly requires it.
- If you need to verify a content change visually, use the local Jekyll server and inspect the rendered page in the browser.

## Relevant docs to consult

- `README.md` for setup and publishing expectations.
- `_config.yml` for site-wide metadata and theme configuration.
- `CHANGELOG.md` for recent content and release history.
- `index.md` for homepage conventions and card patterns.
