---
name: frontend-design
description: This file describes frontend design principles to avoid generic "AI slop" aesthetics.  Use this skill when the user asks to design/build web components or pages or applications.
---
# Frontend Design Instructions

Based on Anthropic's [Improving Frontend Design Through Skills](https://claude.com/blog/improving-frontend-design-through-skills) blog post.

## Core Principle

Avoid "AI slop" aesthetic - the generic, on-distribution outputs that converge toward Inter fonts, purple gradients on white backgrounds, and minimal animations. Make creative, distinctive frontends that surprise and delight.

## Frontend Aesthetics

<frontend_aesthetics>
You tend to converge toward generic, "on distribution" outputs. In frontend design, this creates what users call the "AI slop" aesthetic. Avoid this: make creative, distinctive frontends that surprise and delight.

Focus on:

- **Typography**: Choose fonts that are beautiful, unique, and interesting. Avoid generic fonts like Arial and Inter; opt instead for distinctive choices that elevate the frontend's aesthetics.

- **Color & Theme**: Commit to a cohesive aesthetic. Use CSS variables for consistency. Dominant colors with sharp accents outperform timid, evenly-distributed palettes. Draw from IDE themes and cultural aesthetics for inspiration.

- **Motion**: Use animations for effects and micro-interactions. Prioritize CSS-only solutions for HTML. Use Motion library for React when available. Focus on high-impact moments: one well-orchestrated page load with staggered reveals (animation-delay) creates more delight than scattered micro-interactions.

- **Backgrounds**: Create atmosphere and depth rather than defaulting to solid colors. Layer CSS gradients, use geometric patterns, or add contextual effects that match the overall aesthetic.

Avoid generic AI-generated aesthetics:
- Overused font families (Inter, Roboto, Arial, system fonts)
- Clichéd color schemes (particularly purple gradients on white backgrounds)
- Predictable layouts and component patterns
- Cookie-cutter design that lacks context-specific character

Interpret creatively and make unexpected choices that feel genuinely designed for the context. Vary between light and dark themes, different fonts, different aesthetics. You still tend to converge on common choices (Space Grotesk, for example) across generations. Avoid this: it is critical that you think outside the box!
</frontend_aesthetics>

## Typography Guidelines

<use_interesting_fonts>
Typography instantly signals quality. Avoid using boring, generic fonts.

**Never use**: Inter, Roboto, Open Sans, Lato, default system fonts

**Here are some examples of good, impactful choices**:
- Code aesthetic: JetBrains Mono, Fira Code, Space Grotesk
- Editorial: Playfair Display, Crimson Pro
- Technical: IBM Plex family, Source Sans 3
- Distinctive: Bricolage Grotesque, Newsreader

**Pairing principle**: High contrast = interesting. Display + monospace, serif + geometric sans, variable font across weights.

**Use extremes**: 100/200 weight vs 800/900, not 400 vs 600. Size jumps of 3x+, not 1.5x.

**Pick one distinctive font, use it decisively**. Load from Google Fonts.
</use_interesting_fonts>

## Example: Theme-Based Design

When creating themed designs, commit fully to the aesthetic. Example:

<rpg_theme_example>
Always design with RPG aesthetic:
- Fantasy-inspired color palettes with rich, dramatic tones
- Ornate borders and decorative frame elements
- Parchment textures, leather-bound styling, and weathered materials
- Epic, adventurous atmosphere with dramatic lighting
- Medieval-inspired serif typography with embellished headers
</rpg_theme_example>

## Application to This Project

For this Jekyll blog:
- Current design uses custom inline styling with blue palette (#1e3a5f, #2c5282, #4a6fa5)
- Card-based layouts with gradient headers
- Consider: More distinctive typography choices beyond system defaults
- Consider: Subtle animations for card hover states or page transitions
- Consider: Atmospheric backgrounds instead of solid colors
- Maintain current cohesive color scheme but enhance with depth/texture

## Resources

- [Frontend Design Cookbook](https://github.com/anthropics/claude-cookbooks/blob/main/coding/prompting_for_frontend_aesthetics.ipynb)
- [Claude Code Frontend Design Plugin](https://github.com/anthropics/claude-code/tree/main/plugins/frontend-design)
- [Skills Repository](https://github.com/anthropics/skills)

---

*Source: Anthropic Applied AI team - November 12, 2025*
