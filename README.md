# Zeeshan Altaf — Personal Profile Webpage

Personal portfolio and profile website for **Zeeshan Altaf**, an Agentic AI Architect specializing in AI-powered SaaS applications, Agentic AI workflows, automation workflows, and Agentic RAG systems.

🌐 **Live Site:** _(add your deployment URL here)_

---

## Overview

A clean, premium dark-themed profile webpage built with plain HTML, CSS, and JavaScript — no frameworks, no build tools. Deploy anywhere in seconds.

---

## Sections

| Section | Description |
|---------|-------------|
| **Hero** | Full-viewport introduction with animated gradient background |
| **What I Build** | Four expertise areas: SaaS, Agentic AI, Automation, RAG |
| **AI-Powered Applications** | Showcase of ResuMatchAI, InvoiceExtract, and FitFusion |
| **Automation Workflows** | Multi-Agent Slackbot and YouTube Analytics Pipeline |
| **Contact** | Contact form (Formspree) + social links |

---

## Projects Featured

### AI-Powered Applications

- **[ResuMatchAI](https://resumatch.zeeshanai.cloud)** — AI-powered resume scoring against job descriptions. Tells you exactly what to fix before you apply.
- **[InvoiceExtract](https://invoicextract.zeeshanai.cloud)** — Extracts structured data (line items, totals, vendor details) from PDF/image invoices and returns clean JSON.
- **FitFusion** _(in development)_ — AI-powered workout and nutrition plan generator based on user profile, fitness goals, and training level.

### Automation Workflows

- **Multi-Agent Slackbot** — Custom Slackbot with three specialized AI agents:
  - *Channel Bootstrapping Agent* — Summarizes channel history and indexes uploaded files into a knowledge base
  - *New User On-Boarding Agent* — Briefs new members with project status, stakeholders, and dev process
  - *Ask-Me Agent* — Answers project questions from Slack history and document artifacts (PDF, DOCX, CSV)
- **YouTube Analytics Pipeline** — Tracks channel performance metrics including subscriber growth, view trends, and daily upload cadence.

---

## Tech Stack

| Concern | Technology |
|---------|-----------|
| Markup | HTML5 (semantic) |
| Styling | CSS3 (custom properties, grid, flexbox, `@keyframes`) |
| Interactivity | Vanilla JavaScript (ES6+, IntersectionObserver API) |
| Fonts | [Syne](https://fonts.google.com/specimen/Syne) + [Outfit](https://fonts.google.com/specimen/Outfit) via Google Fonts |
| Contact form | [Formspree](https://formspree.io) |

---

## File Structure

```
profile/
├── index.html      # Semantic HTML5 structure and content
├── style.css       # Design system, layout, animations
├── script.js       # Scroll reveals, active nav, mobile menu
└── README.md
```

---

## Design System

**Color Palette**

| Token | Value | Usage |
|-------|-------|-------|
| Background | `#0a0a0f` | Page base |
| Card surface | `#16161e` | Cards and panels |
| Text primary | `#f0ece6` | Headings and body |
| Text secondary | `#9a958e` | Descriptions |
| Accent | `#e8a838` | Links, highlights, CTA |

**Typography**
- Display / headings: **Syne** (weights 400, 700, 800)
- Body / UI text: **Outfit** (weights 300, 400, 500, 600)

---

## Getting Started

No installation or build step needed. Just open `index.html` in a browser:

```bash
# Clone the repo
git clone https://github.com/mzeeshanaltaf/profile.git
cd profile

# Open directly in browser (macOS / Linux)
open index.html

# Or on Windows
start index.html
```

---

## Deployment

This site can be deployed to any static hosting platform:

### GitHub Pages
1. Push the repository to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your site will be live at `https://<username>.github.io/<repo>`

### Netlify
1. Drag and drop the project folder onto [netlify.com/drop](https://netlify.com/drop)
2. Or connect your GitHub repository in the Netlify dashboard

### Vercel
```bash
npx vercel --prod
```

---

## Configuration

### Contact Form
The form uses [Formspree](https://formspree.io). The endpoint is already configured. To use a different endpoint, update the `action` attribute in [index.html](index.html):

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Social Links
Update the `href` values in the contact section of [index.html](index.html) to point to your profiles.

---

## License

© 2026 Zeeshan Altaf. All rights reserved.
