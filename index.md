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
  - name: Anthropic RED Teaming
    url: https://red.anthropic.com/
    note: Safety evaluations, system cards, and red-team insights
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

<div class="journey-hero reveal-up">
  <h1>Human in the Loop</h1>
  <p>Experiments in coding with AI, from first prompt to finished result.</p>
</div>

## 🚀 Recent Adventures

<div class="adventures-shell reveal-up reveal-up-delay-1">
  <a class="adventure-featured" href="./2026-May-24.html">
    <span class="adventure-featured-badge">Latest Log</span>
    <h3>March Through May Projects</h3>
    <p>Ralph Loop, Copilot Assistant, Codex and Claude workflows, and the LLM Wiki all in one sprint recap.</p>
    <span class="adventure-featured-meta">2026-05-24 • Read entry -></span>
  </a>

  <div class="adventure-timeline" role="list" aria-label="Recent adventures timeline">
    <a class="adventure-row" role="listitem" href="./2026-Mar-08.html"><span class="adventure-date">2026-03-08</span><span class="adventure-main"><span class="adventure-title">Harnessing OpenClaw - Orchestrating Multiple AI Agents</span><span class="adventure-tags"><span class="adventure-tag">AI agents</span><span class="adventure-tag">Orchestration</span></span></span></a>
    <a class="adventure-row" role="listitem" href="./2026-Feb-7.html"><span class="adventure-date">2026-02-07</span><span class="adventure-main"><span class="adventure-title">Home Assistant MCP Server</span><span class="adventure-tags"><span class="adventure-tag">Home automation</span><span class="adventure-tag">MCP</span></span></span></a>
    <a class="adventure-row" role="listitem" href="./2026-Feb-1.html"><span class="adventure-date">2026-02-01</span><span class="adventure-main"><span class="adventure-title">Skills vs Instructions in AI Agent Configuration</span><span class="adventure-tags"><span class="adventure-tag">AI config</span><span class="adventure-tag">Prompting</span></span></span></a>
    <a class="adventure-row" role="listitem" href="./2026-Jan-29.html"><span class="adventure-date">2026-01-29</span><span class="adventure-main"><span class="adventure-title">GitHub Copilot CLI, MCP Apps, Dev Containers</span><span class="adventure-tags"><span class="adventure-tag">Tooling</span><span class="adventure-tag">Devcontainers</span></span></span></a>
    <a class="adventure-row" role="listitem" href="./2026-Jan-17.html"><span class="adventure-date">2026-01-17</span><span class="adventure-main"><span class="adventure-title">Projects - Interactive Web Apps and MCP Tools</span><span class="adventure-tags"><span class="adventure-tag">Web apps</span><span class="adventure-tag">MCP tools</span></span></span></a>
    <a class="adventure-row" role="listitem" href="./2026-Jan-11.html"><span class="adventure-date">2026-01-11</span><span class="adventure-main"><span class="adventure-title">Weekend projects and discoveries</span><span class="adventure-tags"><span class="adventure-tag">Weekend build</span><span class="adventure-tag">Experiments</span></span></span></a>
    <a class="adventure-row" role="listitem" href="./2025-Nov-8.html"><span class="adventure-date">2025-11-08</span><span class="adventure-main"><span class="adventure-title">Jekyll and GitHub Pages setup</span><span class="adventure-tags"><span class="adventure-tag">Jekyll</span><span class="adventure-tag">GitHub Pages</span></span></span></a>
    <a class="adventure-row" role="listitem" href="./2025-Nov.html"><span class="adventure-date">2025-11</span><span class="adventure-main"><span class="adventure-title">WSL Terminal Adventures</span><span class="adventure-tags"><span class="adventure-tag">WSL</span><span class="adventure-tag">CLI</span></span></span></a>
  </div>
</div>

## 🤖 Favorite AI Blogs

<div class="blog-panel reveal-up reveal-up-delay-1">
  <ul>
    {% for blog in page.ai_blogs %}
      <li>
        <a href="{{ blog.url }}" target="_blank" rel="noopener noreferrer">{{ blog.name }}</a>
        <span class="blog-note"> - {{ blog.note }}</span>
      </li>
    {% endfor %}
  </ul>
</div>

## 💡 Project Showcase

<div class="showcase-grid reveal-up reveal-up-delay-2">
  <div class="showcase-card">
    <h3>WSL Terminal Adventures</h3>
    <p>Getting Copilot to explore my WSL terminal setup and configuration.</p>
    <a href="./2025-Nov.html">Read More -></a>
  </div>
  
  <div class="showcase-card">
    <h3>Jekyll and GitHub Pages</h3>
    <p>Implementing Burke Holland's approach to building a blog with Jekyll on GitHub Pages.</p>
    <a href="./2025-Nov-8.html">Read More -></a>
  </div>

  <div class="showcase-card">
    <h3>Rondeau Area OSM Map</h3>
    <p>An interactive OpenStreetMap trip planner for the June-July 2026 Rondeau camping trip.</p>
    <a href="{{ '/Rondeau-Area-OpenStreetMap.html' | relative_url }}">Open Map -></a>
  </div>

  <div class="showcase-card">
    <h3>Switzerland 2026 Dashboard</h3>
    <p>An interactive trip dashboard for itinerary, hotels, flights, and reminders.</p>
    <a href="{{ '/switzerland-dashboard.html' | relative_url }}">Open Dashboard -></a>
  </div>
</div>

## 🧪 Latest Projects (March-May 2026)

<div class="projects-latest reveal-up reveal-up-delay-2">
  <ul>
    <li><strong>Ralph Loop</strong></li>
    <li><strong>Copilot Assistant</strong></li>
    <li><strong>OpenAI Codex and Claude Desktop</strong> (Chat/Cowork/Code)</li>
    <li><strong>LLM Wiki</strong></li>
  </ul>
</div>


---

<div class="home-footer-note">
  <p>✨ Built with Jekyll • Hosted on GitHub Pages • Updated May 2026</p>
</div>


