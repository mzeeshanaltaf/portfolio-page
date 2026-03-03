# Zeeshan Altaf — Profile Webpage

## Context
Create a personal portfolio/profile webpage for Zeeshan Altaf, an AI engineer specializing in AI-powered SaaS applications, Agentic AI workflows, automation, and Agentic RAG. The page showcases projects and automation workflows with a clean, premium aesthetic. No build tools — plain HTML/CSS/JS for easy deployment anywhere.

## File Structure
```
e:/Projects/Claude Code/Profile/
  index.html    — Semantic HTML5, Google Fonts, all content
  style.css     — Styling, animations, responsive breakpoints
  script.js     — IntersectionObserver, scroll behavior, mobile menu
```

## Design System

### Typography (Google Fonts)
- **Display (headings/hero):** Syne — weights 400, 700, 800
- **Body:** Outfit — weights 300, 400, 500, 600
- Hero name: `clamp(2.75rem, 5.5vw, 5rem)` Syne 800 _(scaled down from original for better balance)_

### Color Palette (Dark + Amber Accent)
| Token | Value | Use |
|-------|-------|-----|
| `--color-bg-primary` | `#0a0a0f` | Page background |
| `--color-bg-card` | `#16161e` | Card surfaces |
| `--color-text-primary` | `#f0ece6` | Headings, body text |
| `--color-text-secondary` | `#9a958e` | Descriptions |
| `--color-accent` | `#e8a838` | Links, highlights, CTA |

### Animations
- Hero: staggered `fadeInUp` on page load (eyebrow → name → tagline)
- Sections: scroll-triggered `reveal` via IntersectionObserver (opacity + translateY)
- Cards: hover lift (`translateY(-6px)`) + border glow
- Background: CSS gradient mesh drifting slowly behind hero
- Navbar: always visible, fixed to top _(updated from original hide-on-scroll)_
- `prefers-reduced-motion` respected

## Sections

### 1. Fixed Navigation
- Frosted glass header (`backdrop-filter: blur`)
- "ZA" monogram (accent) + nav links (About, Projects, Automation, Contact)
- Hamburger menu on mobile → fullscreen overlay
- Always stays visible while scrolling

### 2. Hero (100vh)
- Eyebrow: "Agentic AI Architect | AI-Driven Business Automation" (accent, uppercase, tracked)
- Name: "Zeeshan Altaf" (Syne 800)
- Tagline: "Building autonomous AI systems, agentic workflows & intelligent automation."
- Animated gradient mesh background (CSS-only)
- Scroll indicator with pulsing dot

### 3. Expertise ("What I Build")
- Intro paragraph + 2x2 grid of cards:
  1. AI-Powered SaaS Applications
  2. Agentic AI Workflows
  3. Automation Workflows
  4. Agentic RAG
- Watermark numbers (01–04) as decorative elements

### 4. AI-Powered Applications
- 2-column project cards:
  - **ResuMatchAI** — Resume scoring/matching → `https://resumatch.zeeshanai.cloud`
  - **InvoiceExtract** — PDF/image invoice extraction → `https://invoicextract.zeeshanai.cloud`
  - **FitFusion** — Workout & nutrition planner → "Coming Soon" (no link)
- Each card: title, description, "View Project →" link with hover arrow shift

### 5. Automation Workflows
- Full-width stacked cards with left accent border:
  - **Multi-Agent Slackbot** — with 3 sub-agents listed (Channel Bootstrapping, Onboarding, Ask-Me)
  - **YouTube Analytics Pipeline** — channel tracking, subscriber/view metrics

### 6. Contact ("Get In Touch")
- Asymmetric 2-column: form (60%) + social links (40%)
- Form: Name, Email, Message, Submit → Formspree (`https://formspree.io/f/mvzbjybq`)
- Social links: GitHub, LinkedIn, Twitter/X, Email (with real URLs)

### 7. Footer
- Minimal: "© 2026 Zeeshan Altaf. All rights reserved."

## Responsive Breakpoints (Mobile-First)
- Default: single-column, stacked cards, hamburger nav
- `768px`: 2-column grids, inline nav
- `1024px`: full layout, larger spacing
- `1400px`: content capped at 1200px centered

## Accessibility
- Skip-to-content link
- Semantic landmarks (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`)
- `aria-label` on sections, `aria-expanded` on menu toggle
- WCAG AA+ contrast ratios verified
- `prefers-reduced-motion` disables all animations
- Form inputs with proper `<label>` associations

## Post-Build Changes
| Change | File |
|--------|------|
| Navbar always visible (removed hide-on-scroll) | `script.js`, `style.css` |
| Hero name scaled down; eyebrow/tagline weight increased | `style.css` |
| Updated hero eyebrow and tagline copy | `index.html` |
| Formspree endpoint set to real form ID | `index.html` |
| Social links updated with real profile URLs | `index.html` |

## Implementation Order
1. `index.html` — full HTML structure with all content and class names
2. `style.css` — CSS variables → reset → navigation → hero → sections → cards → contact → responsive → animations
3. `script.js` — IntersectionObserver, navbar scroll, mobile menu, smooth scroll, active link

## Verification
- Open `index.html` directly in browser to test (no server needed)
- Resize browser to test responsive breakpoints (mobile/tablet/desktop)
- Verify all project links work (resumatch, invoicextract)
- Test contact form (Formspree endpoint is live)
- Check scroll animations trigger properly
- Test keyboard navigation and skip link
