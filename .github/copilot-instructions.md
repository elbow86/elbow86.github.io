# Copilot Instructions for elbow86.github.io

## Project Overview

Personal tech blog and portfolio built with **Jekyll 4.4.1** and hosted on **GitHub Pages**. This is a minimal setup with blog posts as root-level Markdown files and custom inline styling.

## Architecture & Structure

```
elbow86.github.io/
├── index.md              # Landing page with custom HTML/CSS cards
├── _config.yml           # Jekyll config (Minima theme)
├── YYYY-MMM-DD.md        # Blog posts (date-based naming)
├── CHANGELOG.md          # Manual changelog
├── _site/                # Generated output (git-ignored)
└── vendor/               # Ruby dependencies
```

**Key Point**: Blog posts live at root level, not in `_posts/` directory. Jekyll converts them to HTML using the `page` layout.

## Development Workflow

### Starting the Local Server

```bash
cd /workspaces/repos/pages/elbow86.github.io
bundle exec jekyll serve --livereload
```

- Server runs on `http://127.0.0.1:4000`
- Press Ctrl+C to stop
- Clear cache if issues: `bundle exec jekyll clean`

### Adding a New Blog Post

1. **Create file** with date-based naming:
   - Format: `YYYY-MMM-DD.md` (e.g., `2026-Feb-01.md`)
   - Or: `YYYY-MMM.md` for monthly summaries

2. **Use this frontmatter template**:
   ```markdown
   ---
   layout: page
   title: Your Post Title Here
   ---
   # Your Post Title
   
   Your content here...
   ```

3. **Update [`index.md`](index.md)** - Add card to "Recent Adventures" section:
   ```html
   <div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px; border-left: 4px solid #2c5282; margin-bottom: 1.5rem;">
     <h3 style="margin-top: 0; color: #1e3a5f;">📅 <a href="./2026-Feb-01.html">February 1, 2026</a></h3>
     <p style="margin-bottom: 0; color: #6c757d;">Brief description</p>
   </div>
   ```

4. **Update [`CHANGELOG.md`](CHANGELOG.md)** with the new post details

## Critical Conventions

### File Naming
- Blog posts: `YYYY-MMM-DD.md` (e.g., `2026-Jan-29.md`)
- **NO underscores or `_posts/` directory** - posts are root-level files

### Internal Linking
- Use `.html` extension, not `.md`: `[Link](./2026-Jan-29.html)`
- Jekyll converts `.md` to `.html` during build
- Relative paths: `./filename.html`

### Styling
Custom inline styling with blue color palette:
- Primary: `#1e3a5f`
- Secondary: `#2c5282`
- Accent: `#4a6fa5`
- Card backgrounds: `#f8f9fa` with colored left borders
- See [`index.md`](index.md) for card and gradient header examples

### Layouts
- Blog posts use: `layout: page`
- Home page uses: `layout: home`
- Theme is Minima 2.5.2 (see [`_config.yml`](_config.yml))

## Deployment

- **Automatic**: Push to `main` branch triggers GitHub Pages deployment
- **Live in 1-2 minutes** at https://elbow86.github.io
- Check "Actions" tab for build status

## Common Tasks

**Update site title/description**: Edit [`_config.yml`](_config.yml)

**Modify homepage layout**: Edit [`index.md`](index.md) (custom HTML/CSS embedded)

**View recent changes**: Check [`CHANGELOG.md`](CHANGELOG.md)

**Rebuild site**: `bundle exec jekyll build`

## Known Patterns

- **Manual index updates**: No automation - must manually add cards to `index.md` when creating posts
- **Changelog discipline**: Update `CHANGELOG.md` for all content changes
- **External projects**: Links to external demos (moonunit.ca domain) in Project Showcase section
- **Date consistency**: File names must match post titles/dates
