---
layout: home
ai_blogs:

  - name: Burke Holland
    url: https://burkeholland.github.io/
    note: Developer insights and learning journeys

  - name: OpenAI News
    url: https://openai.com/news/
    note: Model updates and product releases
  - name: OpenAI Developers Blog
    url: https://developers.openai.com/blog
    note: OpenAI platform and API updates
  - name: OpenAI Codex
    url: https://developers.openai.com/blog/topic/codex
    note: AI code generation and Codex updates

  - name: Anthropic News
    url: https://www.anthropic.com/news
    note: Research and product posts
  - name: Claude Blog
    url: https://claude.com/blog
    note: Anthropic Claude product announcements

  - name: Hugging Face Blog
    url: https://huggingface.co/blog
    note: Open-source AI ecosystem updates
  - name: Simon Willison
    url: https://simonwillison.net/
    note: Practical AI tooling and experiments
  - name: Latent Space
    url: https://www.latent.space/
    note: Deep dives on LLM engineering
---

<div style="text-align: center; padding: 2rem 0; background: linear-gradient(135deg, #1e3a5f 0%, #2c5282 100%); color: white; border-radius: 10px; margin-bottom: 2rem;">
  <h1 style="margin: 0; font-size: 2.5rem; font-weight: bold;">👋 Tech Journey</h1>
  <p style="font-size: 1.2rem; margin-top: 1rem; opacity: 0.95;">...</p>
</div>

## 🚀 Recent Adventures

<div style="background: #f8f9fa; padding: 0.9rem 1rem; border-radius: 8px; border-left: 4px solid #0d2847; margin-bottom: 0.8rem;">
  <p style="margin: 0; font-size: 0.9rem; color: #333;">📅 <a href="./2026-Mar-08.html" style="color: #0d2847; text-decoration: none; font-weight: 500;">March 8, 2026</a> — Harnessing OpenClaw - Orchestrating Multiple AI Agents</p>
</div>

<div style="background: #f8f9fa; padding: 0.9rem 1rem; border-radius: 8px; border-left: 4px solid #1e3a5f; margin-bottom: 0.8rem;">
  <p style="margin: 0; font-size: 0.9rem; color: #333;">📅 <a href="./2026-Feb-7.html" style="color: #1e3a5f; text-decoration: none; font-weight: 500;">February 7, 2026</a> — Home Assistant MCP Server</p>
</div>

<div style="background: #f8f9fa; padding: 0.9rem 1rem; border-radius: 8px; border-left: 4px solid #1e3a5f; margin-bottom: 0.8rem;">
  <p style="margin: 0; font-size: 0.9rem; color: #333;">📅 <a href="./2026-Feb-1.html" style="color: #1e3a5f; text-decoration: none; font-weight: 500;">February 1, 2026</a> — Skills vs Instructions in AI Agent Configuration</p>
</div>

<div style="background: #f8f9fa; padding: 0.9rem 1rem; border-radius: 8px; border-left: 4px solid #2c5282; margin-bottom: 0.8rem;">
  <p style="margin: 0; font-size: 0.9rem; color: #333;">📅 <a href="./2026-Jan-29.html" style="color: #1e3a5f; text-decoration: none; font-weight: 500;">Jan 29-Feb 1, 2026</a> — GitHub Copilot CLI, MCP Apps, Dev Containers</p>
</div>

<div style="background: #f8f9fa; padding: 0.9rem 1rem; border-radius: 8px; border-left: 4px solid #4a6fa5; margin-bottom: 0.8rem;">
  <p style="margin: 0; font-size: 0.9rem; color: #333;">📅 <a href="./2026-Jan-17.html" style="color: #1e3a5f; text-decoration: none; font-weight: 500;">January 17, 2026</a> — Projects - Interactive Web Apps & MCP Tools</p>
</div>

<div style="background: #f8f9fa; padding: 0.9rem 1rem; border-radius: 8px; border-left: 4px solid #6c9bd1; margin-bottom: 0.8rem;">
  <p style="margin: 0; font-size: 0.9rem; color: #333;">📅 <a href="./2026-Jan-11.html" style="color: #1e3a5f; text-decoration: none; font-weight: 500;">Weekend of January 10-11, 2026</a> — Weekend projects and discoveries</p>
</div>

<div style="background: #f8f9fa; padding: 0.9rem 1rem; border-radius: 8px; border-left: 4px solid #8ba8c7; margin-bottom: 0.8rem;">
  <p style="margin: 0; font-size: 0.9rem; color: #333;">📅 <a href="./2025-Nov-8.html" style="color: #2c5282; text-decoration: none; font-weight: 500;">November 8, 2025</a> — Jekyll & GitHub Pages setup</p>
</div>

<div style="background: #f8f9fa; padding: 0.9rem 1rem; border-radius: 8px; border-left: 4px solid #9db5d1; margin-bottom: 0.8rem;">
  <p style="margin: 0; font-size: 0.9rem; color: #333;">📅 <a href="./2025-Nov.html" style="color: #1e3a5f; text-decoration: none; font-weight: 500;">November 2025</a> — WSL Terminal Adventures</p>
</div>

## 🤖 Favorite AI Blogs

<div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px; border-left: 4px solid #0d2847; margin-bottom: 2rem;">
  <ul style="margin: 0; padding-left: 1.2rem;">
    {% for blog in page.ai_blogs %}
      <li style="margin-bottom: 0.7rem;">
        <a href="{{ blog.url }}" target="_blank" rel="noopener noreferrer">{{ blog.name }}</a>
        <span style="color: #6c757d;"> - {{ blog.note }}</span>
      </li>
    {% endfor %}
  </ul>
</div>

## 💡 Project Showcase

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem; margin-top: 1rem;">
  <div style="background: white; padding: 1.5rem; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1); border-top: 3px solid #2c5282;">
    <h3 style="margin-top: 0; color: #1e3a5f;">🖥️ WSL Terminal Adventures</h3>
    <p style="color: #6c757d;">Getting Copilot to explore my WSL Terminal setup and configuration</p>
    <a href="./2025-Nov.html" style="color: #2c5282; text-decoration: none; font-weight: bold;">Read More →</a>
  </div>
  
  <div style="background: white; padding: 1.5rem; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1); border-top: 3px solid #4a6fa5;">
    <h3 style="margin-top: 0; color: #2c5282;">📝 Jekyll & GitHub Pages</h3>
    <p style="color: #6c757d;">Implementing Burke Holland's approach to building a blog with Jekyll on GitHub Pages</p>
    <a href="./2025-Nov-8.html" style="color: #4a6fa5; text-decoration: none; font-weight: bold;">Read More →</a>
  </div>
</div>

## 🛠️ What I'm Working On

- Exploring AI-powered development tools
- Building with Jekyll and GitHub Pages
- Terminal customization and productivity
- Documenting recent learning journey

---

<div style="text-align: center; padding: 1rem; color: #6c757d; font-size: 0.9rem;">
  <p>✨ Built with Jekyll • Hosted on GitHub Pages • Updated January 2026</p>
</div>


