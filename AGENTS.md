# AGENTS.md

## Project overview

This repository is a personal blog and project portfolio built with Jekyll and hosted on GitHub Pages. It is a static site project focused on Markdown content and custom page markup, not an application backend.

## Build and validation commands

Run from the repository root:

```bash
bundle install
bundle exec jekyll build
bundle exec jekyll serve --livereload
```

- Use `bundle exec jekyll build` as the default validation step for changes.
- Use `bundle exec jekyll serve --livereload` for local preview at `http://127.0.0.1:4000`.
- If build output looks stale, run `bundle exec jekyll clean` and rebuild.
- There is no dedicated unit-test/lint pipeline in this repo; build success is the primary correctness signal.

## High-level architecture

- `_config.yml` defines site metadata and core Jekyll behavior.
- `index.md` is the homepage and includes custom HTML/CSS sections plus front matter.
- Blog content is stored as root-level Markdown files (for example `2026-Jan-29.md`, `2026-Feb-1.md`) rather than `_posts/`.
- Jekyll converts Markdown pages to HTML at build time.
- `_site/` is generated output and should not be manually edited.
- `vendor/` contains Ruby dependencies for local development.

## Repository-specific conventions

### Content and naming
- Keep posts at the repository root.
- Use date-based filenames (`YYYY-MMM-DD.md` or `YYYY-MMM.md`).
- Keep filename, title, and visible post date aligned.

### Front matter and layouts
Use this structure for standard entries:

```yaml
---
layout: page
title: Your Post Title
---

# Your Post Title
```

- Use `layout: page` for post pages.
- Keep `index.md` on its existing `layout: home` pattern.

### Linking
- Link to generated HTML routes (example: `./2026-Jan-29.html`) rather than source `.md` links for published navigation.
- Keep relative-link style consistent with existing pages.

### Update flow for new/edited posts
When content changes:
- Update homepage cards/timeline in `index.md` when applicable.
- Update `CHANGELOG.md` for user-visible additions/changes.

### Styling
- Preserve the current inline-heavy styling approach and existing palette (`#1e3a5f`, `#2c5282`, `#4a6fa5`).
- Reuse current card/timeline patterns instead of introducing unrelated visual systems.

### User-level journal tracking

- Maintain a user-level journal at `/workspace/JOURNAL.md` for personal notes, experiments, and session learnings.
- When a user asks for a recap, a blog post, or a meaningful workflow review, update the journal with a dated summary of what happened.
- Keep the journal in a lightweight, practical format: outcome, prompt/tool context, and next step or follow-up.
- Use the journal as the personal memory layer that complements the repo changelog.

## Primary reference files

- `README.md`
- `_config.yml`
- `index.md`
- `CHANGELOG.md`
- `.github/copilot-instructions.md`
- `/workspace/JOURNAL.md`
