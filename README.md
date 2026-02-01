# elbow86.github.io

Personal tech blog and project portfolio powered by Jekyll and GitHub Pages.

## 🚀 Overview

This site documents my tech journey, projects, and explorations across various technologies including:
- AI-powered development tools (GitHub Copilot, MCP Apps)
- Interactive web projects (Solar System simulator, games, visualizations)
- Development workflows (Jekyll, Dev Containers, WSL)
- Infrastructure experiments (Docker, Kubernetes, Minecraft servers)

**Live Site**: https://elbow86.github.io

## 🛠️ Tech Stack

- **Static Site Generator**: Jekyll 4.4.1
- **Theme**: Minima 2.5.2
- **Hosting**: GitHub Pages
- **Ruby**: 3.3.0
- **Markup**: Markdown with custom inline styling

## 📁 Project Structure

```
elbow86.github.io/
├── index.md              # Main landing page with styled sections
├── _config.yml           # Jekyll configuration
├── CHANGELOG.md          # Project changelog
├── README.md             # This file
├── 2026-Jan-*.md         # Blog posts (date-based naming)
├── 2025-Nov-*.md         # Older blog posts
├── _site/                # Generated site (git-ignored)
└── vendor/               # Ruby dependencies
```

## 🖥️ Local Development

### Prerequisites

- Ruby 3.x
- Bundler
- Jekyll (installed via Bundler)

### Setup & Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/elbow86/elbow86.github.io.git
   cd elbow86.github.io
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Serve locally**
   ```bash
   bundle exec jekyll serve
   ```
   
   Or with live reload:
   ```bash
   bundle exec jekyll serve --livereload
   ```

4. **Preview in browser**
   - Open [http://127.0.0.1:4000](http://127.0.0.1:4000)
   - Or if using a different port: http://127.0.0.1:4001

5. **Build only (no server)**
   ```bash
   bundle exec jekyll build
   ```

### Development Tips

- Jekyll watches for file changes and rebuilds automatically
- Press `Ctrl+C` to stop the server
- Clear the cache if you encounter issues: `bundle exec jekyll clean`

## ✍️ Adding New Posts

### File Naming Convention

Use date-based naming for consistency:
- Format: `YYYY-MMM-DD.md` (e.g., `2026-Jan-29.md`)
- Or: `YYYY-MMM.md` for monthly summaries (e.g., `2025-Nov.md`)

### Post Template

```markdown
---
layout: page
title: Your Post Title
---

# Your Post Title

Your content here...
```

### Adding to Index

Update `index.md` to add your new post to the "Recent Adventures" section:

```html
<div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px; border-left: 4px solid #2c5282; margin-bottom: 1.5rem;">
  <h3 style="margin-top: 0; color: #1e3a5f;">📅 <a href="./your-file.html">Your Title</a></h3>
  <p style="margin-bottom: 0; color: #6c757d;">Brief description</p>
</div>
```

## 🔗 Internal Linking

- Use relative paths: `./filename.html` (Jekyll converts `.md` to `.html`)
- Markdown links: `[Link Text](./filename.html)`
- Update `CHANGELOG.md` when adding new posts

## 🎨 Styling

The site uses custom inline styling with a blue color scheme:
- Primary: `#1e3a5f`
- Secondary: `#2c5282`
- Accent: `#4a6fa5`
- Gradient headers and card-based layouts

## 🚢 Deployment

This site uses GitHub Pages for automatic deployment:

1. **Push changes** to the `main` branch
2. **GitHub Actions** automatically builds and deploys
3. **View live** at https://elbow86.github.io (typically within 1-2 minutes)

### Viewing Build Status

Check the "Actions" tab in the GitHub repository to see build/deploy status.

## 📝 Blog Posts

### Recent Posts
- **2026-Jan-29**: GitHub Copilot CLI, MCP Apps, Dev Containers
- **2026-Jan-17**: Published Projects (Meditation, Solar System, etc.)
- **2026-Jan-11**: Solar System simulator, Commute calculator, Subscription tracker
- **2025-Nov-8**: Jekyll & GitHub Pages setup
- **2025-Nov**: WSL Terminal exploration

### External Projects
- [Solar System Simulator](https://moonunit.ca/solar/index.html)
- [Meditation App](https://moonunit.ca/meditation/meditation.html)
- [Flow Field Visualization](https://moonunit.ca/meditation/flow-field.html)
- [Squirrel Game](https://moonunit.ca/squirrel/index.html)
- [Ball Physics Demo](https://moonunit.ca/ball/index.html)
- [Commute Simulator](https://moonunit.ca/commute-simulator/index.html)

## 📖 Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Burke Holland's Guide](https://burkeholland.github.io/posts/gh-pages-best-blog/) (inspiration for this setup)

## 📋 Changelog

See [CHANGELOG.md](./CHANGELOG.md) for a detailed history of changes.

## 📄 License

See [LICENSE](./LICENSE) for details.

---

**Last Updated**: February 2026
