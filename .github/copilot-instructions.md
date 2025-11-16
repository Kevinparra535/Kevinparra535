# GitHub Profile Repository Guidelines

## Repository Purpose
This is a **GitHub profile README repository** (username/username pattern) that displays on Kevin Parra's GitHub profile page. It showcases professional work, creative experiments, and hackathon projects through rich markdown and visual storytelling.

## Content Structure & Philosophy

### Visual-First Storytelling
- **Banner:** `./images/banner_github.png` sets the creative tone at the top
- **Project Cards:** Use styled HTML tables (not CSS) with embedded images, descriptions, and tech tags
- **GIFs over static images:** Prefer animated GIFs to show interactive/dynamic projects (`labs_*.gif`, `professional_*.gif`, `hackathon_*.gif`)

### Sections (maintain this order)
1. **Header:** Banner + social badges (LinkedIn, Portfolio, Gmail, Instagram, HackerRank)
2. **About Me:** Creative Technologist positioning, location, current focus, tech stack, work approach
3. **Creative Labs:** WebGL/3D experiments (React Three Fiber, GLSL, Three.js)
4. **Hackathons:** 24-48hr rapid prototyping projects showcasing speed + craft
5. **Professional Work:** Client/production projects with business context
6. **GitHub Stats:** Auto-generated stats widgets

## Key Patterns & Conventions

### Tech Tag System
Always wrap technologies in `<code>` tags within project cards:
```html
<code>React Three Fiber</code> <code>GLSL3</code> <code>TypeScript</code>
```

Common tags by category:
- **Creative/3D:** React Three Fiber, GLSL3, ThreeJS, Blender, WebGL, React Three Drei, React Three PostProcessing
- **Frontend:** React, Next.js, TypeScript, Vite, Styled-Components
- **Mobile:** React Native, Firebase
- **Architecture:** SOLID, Clean Architecture, MobX, Zustand, InversifyJS
- **Backend/Real-time:** Node.js, Socket.IO, Express

### Project Card Template (HTML Table)
```html
<td align="center" width="33%">
  <a class="lab-card" href="[REPO_OR_LIVE_URL]" target="_blank" style="[INLINE_STYLES]">
    <img src="/images/[PROJECT_IMAGE].gif" alt="[ALT_TEXT]" style="width:100%; aspect-ratio:16/9; object-fit:cover;">
    <div style="padding:12px 14px; text-align:left;">
      <h4 style="margin:0 0 6px 0;">[PROJECT_NAME]</h4>
      <p style="margin:0 0 8px 0; font-size:14px; line-height:1.4;">
        [CONCISE_DESCRIPTION_FOCUSING_ON_OUTCOME_OR_UNIQUE_ASPECT]
      </p>
      <p style="margin:0; font-size:12px;">
        [TECH_TAGS]
      </p>
    </div>
  </a>
</td>
```

### Writing Style
- **Bold emphasis** on key concepts (e.g., "breathes, reacts and anticipates")
- Quote blocks for personal philosophy statements
- First person, conversational but professional
- Focus on **what makes each project unique** rather than generic descriptions
- Use em-dashes (—) for emphasis

## Adding New Projects

### Before Adding
1. Create a GIF/image in `/images/` directory following naming:
   - `labs_[projectname].gif` for Creative Labs
   - `hackathon_[projectname].gif` for Hackathons
   - `professional_[projectname].gif` or `.jpeg/.png` for Professional Work
2. Ensure aspect ratio is roughly 16:9 for visual consistency

### Placement Logic
- **Creative Labs** = Personal experiments, shaders, WebGL, generative art
- **Hackathons** = Time-constrained builds (24-48hrs), usually full-stack MVPs
- **Professional Work** = Client projects, production apps, commercial work

### Description Guidelines
- Lead with the **"so what?"** — what does it do, who is it for, what's unique?
- Keep to 1-2 sentences (30-50 words max)
- Avoid generic phrases like "cutting-edge" or "innovative" — show, don't tell
- For hackathons, mention time constraint and any constraints/themes

## Asset Management

### Images Directory
All visual assets live in `/images/` with clear naming:
- `banner_github.png` — Profile header banner
- `labs_*.gif` — Creative experiments showcases
- `hackathon_*.gif` — Hackathon project demos
- `professional_*.[gif|jpeg|png]` — Professional work screenshots

### Social Links
Update badges in header section when platforms change. Current active:
- LinkedIn, Portfolio (links.kevcoder.co), Gmail, Instagram, HackerRank

## Maintenance Tasks

### Regular Updates
- Add new projects to appropriate section (Labs/Hackathons/Professional)
- Ensure visitor badge URL matches current repo structure
- Keep "Currently exploring" line in About Me fresh (update quarterly)
- Verify all external links (portfolio, social profiles) remain valid

### Quality Checks
- Test all project links open correctly
- Verify images load properly (use relative paths: `/images/filename.gif`)
- Ensure HTML table structure remains valid (equal column widths, proper nesting)
- Check GitHub stats widgets render correctly

## Philosophy & Voice
Kevin positions himself as a **Creative Technologist** — not just a developer. Emphasize:
- **Art + computation** intersection
- **High-pressure environments** (hackathons) as a creative strength
- **Process of creating** as core motivation (see quote at top)
- **Product-minded**, **performance-focused**, **design-driven** approach

When writing for this profile, blend technical credibility with creative ambition.
