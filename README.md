<div align="center">

<!-- Banner -->
<img src="https://0.gravatar.com/avatar/a2dae9a29fbf7c72552047efc744be54a018938aacd9009e7500f93d72eb0f2e?size=120" width="120" height="120" style="border-radius:50%" alt="Moe Kyaw Aung"/>

# 🌟 Moe Kyaw Aung — Portfolio V3

### `Android Senior Developer · Microsoft Stack · Myanmar`

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-View_Portfolio-d4a843?style=for-the-badge&labelColor=1a1a1a)](https://dev-moe-kyawaung.github.io/Moekyawaung-portfolios-V3)
[![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-Deployed-success?style=for-the-badge&logo=github&logoColor=white&labelColor=1a1a1a)](https://dev-moe-kyawaung.github.io/Moekyawaung-portfolios-V3)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge&labelColor=1a1a1a)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-Pure-E34F26?style=for-the-badge&logo=html5&logoColor=white&labelColor=1a1a1a)](index.html)

---

> *"Building reliable, secure, and user-friendly mobile applications — one commit at a time."*

</div>

---

## 📋 Table of Contents

- [✨ Overview](#-overview)
- [🎨 Design System](#-design-system)
- [📦 Features](#-features)
- [🗂️ Project Structure](#️-project-structure)
- [🚀 Deployment](#-deployment)
- [🛠️ Local Development](#️-local-development)
- [🧩 Tech Stack](#-tech-stack)
- [📸 Screenshots](#-screenshots)
- [📬 Contact](#-contact)
- [📄 License](#-license)

---

## ✨ Overview

**Moekyawaung-portfolios-V3** is a complete, production-ready personal portfolio and landing page for **Moe Kyaw Aung**, a Senior Android Developer based in Tachileik, Myanmar.

Built as a single, self-contained `index.html` file, it requires zero dependencies, zero build tools, and zero frameworks — just open it in a browser or deploy it to any static host.

| Attribute | Detail |
|-----------|--------|
| 👤 **Owner** | Moe Kyaw Aung |
| 🏷️ **Version** | V3 |
| 📍 **Location** | Tachileik, Shan State, Myanmar |
| 🕐 **Timezone** | GMT+07:00 |
| 📧 **Email** | moekyawaung@fastmail.com |
| 📱 **Phone** | +959 666 000 050 |
| 💼 **Role** | Senior Android Developer · Microsoft Stack |

---

## 🎨 Design System

### Visual Identity

| Token | Value | Preview |
|-------|-------|---------|
| Primary Gold | `#d4a843` | 🟡 |
| Gold Light | `#f0c96a` | 🌟 |
| Gold Dark | `#a87e28` | 🟤 |
| Background | `#1a1a1a` | ⬛ |
| Surface | `#242424` | |
| Text Primary | `#f5f0e8` | |
| Text Muted | `#a89880` | |

### Typography

| Role | Font | Weight |
|------|------|--------|
| Display / Headings | Cinzel Decorative | 700, 900 |
| Body / UI | DM Sans | 300–700 |
| Code / Mono | JetBrains Mono | 400, 500 |

### Design Direction

**Glasspunk / Transparent Luxury** — Layered glass panels, gold accents on a deep charcoal base. Vivid, energetic, bold. Every surface breathes with `backdrop-filter: blur()` and subtle gold borders.

---

## 📦 Features

### 🖼️ Sections (5 Pages in One)

| # | Section | Description |
|---|---------|-------------|
| 1 | **Hero** | Animated particle canvas, profile card, social links |
| 2 | **About** | Bio, skill bars, contact info |
| 3 | **Projects** | 6 featured GitHub projects |
| 4 | **Gallery + Certifications** | Lightbox gallery + 12-card carousel |
| 5 | **Pricing + FAQ + Contact** | Service packages, accordion FAQ, validated form |

### ⚡ Interactive Features

- [x] 🎨 **Dark / Light mode toggle** — persistent via CSS variables
- [x] 🍔 **Hamburger-only navigation** — animated slide drawer
- [x] ✨ **Particle canvas hero** — mouse-interactive WebGL-style particles
- [x] 📜 **Scroll-triggered animations** — fade in from left, right, bottom
- [x] 📊 **Animated statistics counters** — smooth number counting
- [x] 🎠 **Certifications carousel** — auto-advancing with dot navigation
- [x] 🖼️ **Image lightbox gallery** — click to zoom, keyboard dismissal
- [x] 💰 **Pricing table** — 3-tier service packages with featured card
- [x] ❓ **FAQ accordion** — smooth expand/collapse with ARIA
- [x] 📬 **Contact form** — full client-side validation + success state
- [x] 📰 **Newsletter form** — email subscription with feedback
- [x] 🗺️ **Google Maps embed** — Tachileik, Myanmar location
- [x] ⬆️ **Back-to-top button** — scroll-aware visibility
- [x] 📌 **Sticky CTA button** — "Hire Me" fixed action button
- [x] ⏳ **Preloader animation** — branded loading screen
- [x] 🌐 **Parallax scrolling** — depth-based layered backgrounds
- [x] 📱 **Fully responsive** — mobile, tablet, desktop

### ♿ Accessibility & SEO

- Semantic HTML5 elements (`<main>`, `<nav>`, `<section>`, `<article>`, `<footer>`)
- ARIA labels on all interactive elements
- `role` attributes on dialogs, navigation, forms
- `sr-only` class for screen-reader-only content
- Open Graph meta tags for social sharing
- Descriptive `alt` text on all images
- Keyboard navigation support (Escape to close lightbox/drawer)
- Focus management on interactive components

---

## 🗂️ Project Structure

```
Moekyawaung-portfolios-V3/
│
├── 📄 index.html                    # Main portfolio (self-contained)
│
├── 📁 assets/
│   ├── css/
│   │   └── README.md                # Note: styles are inline in index.html
│   ├── js/
│   │   └── README.md                # Note: scripts are inline in index.html
│   └── images/
│       └── README.md                # Placeholder for future local assets
│
├── 📁 docs/
│   ├── DESIGN_SYSTEM.md             # Full design token reference
│   ├── DEPLOYMENT.md                # Deployment guide (Pages, Netlify, Vercel)
│   └── CUSTOMIZATION.md             # How to personalize the portfolio
│
├── 📁 .github/
│   ├── workflows/
│   │   └── deploy.yml               # Auto-deploy to GitHub Pages
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.md
│       └── feature_request.md
│
├── 📄 .gitignore                    # Ignore common temp files
├── 📄 LICENSE                       # MIT License
├── 📄 CHANGELOG.md                  # Version history
├── 📄 CONTRIBUTING.md               # Contribution guidelines
└── 📄 README.md                     # This file
```

---

## 🚀 Deployment

### Option 1 — GitHub Pages (Recommended)

The repo includes a pre-configured **GitHub Actions workflow** that auto-deploys on every push to `main`.

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to **GitHub Actions**
4. Push to `main` — the site deploys automatically

**Live URL pattern:** `https://dev-moe-kyawaung.github.io/Moekyawaung-portfolios-V3`

### Option 2 — Netlify (One-click)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Dev-moe-kyawaung/Moekyawaung-portfolios-V3)

1. Click the button above
2. Authorize Netlify with GitHub
3. Deploy — done in under 60 seconds

### Option 3 — Vercel

```bash
npm i -g vercel
vercel deploy
```

### Option 4 — Manual / Any Static Host

Upload `index.html` (and optionally the `assets/` folder) to any web host. No server-side processing required.

---

## 🛠️ Local Development

No build tools or package managers required. Just open the file:

```bash
# Clone the repository
git clone https://github.com/Dev-moe-kyawaung/Moekyawaung-portfolios-V3.git

# Navigate into the project
cd Moekyawaung-portfolios-V3

# Open directly in browser (macOS)
open index.html

# Open directly in browser (Linux)
xdg-open index.html

# Open directly in browser (Windows)
start index.html
```

For live-reload during editing, use VS Code with the **Live Server** extension, or:

```bash
# Using Python (Python 3)
python -m http.server 8080

# Then visit: http://localhost:8080
```

---

## 🧩 Tech Stack

| Technology | Purpose | CDN / Source |
|------------|---------|-------------|
| **HTML5** | Structure & semantics | Native |
| **CSS3** | Styling, animations, variables | Native |
| **Vanilla JavaScript** | Interactivity, DOM, Canvas API | Native |
| **Lucide Icons** | UI icon set | `unpkg.com/lucide` |
| **Google Fonts** | Cinzel Decorative, DM Sans, JetBrains Mono | `fonts.googleapis.com` |
| **Picsum Photos** | Placeholder gallery images | `picsum.photos` |
| **Google Maps** | Location embed | `maps.google.com` |
| **Gravatar** | Developer profile photo | `gravatar.com` |

**Zero npm packages. Zero build steps. Zero runtime frameworks.**

---

## 📸 Screenshots

| Section | Preview |
|---------|---------|
| Hero (Dark) | Animated particle canvas with glasspunk profile card |
| About | Skill bars with smooth width animation |
| Projects | 6-card grid with hover glass reveal |
| Certifications | Auto-advancing carousel (12 certs) |
| Pricing | 3-tier table with gold "Popular" badge |
| Contact | Validated form + Google Maps embed |

> **Note:** Screenshots will be added after the first deployment. See the live demo for a full interactive preview.

---

## 📬 Contact

<div align="center">

| Platform | Link |
|----------|------|
| 📧 Email | [moekyawaung@fastmail.com](mailto:moekyawaung@fastmail.com) |
| 📱 Phone | [+959 666 000 050](tel:+959666000050) |
| 💼 LinkedIn | [moe-kyaw-aung-2653093a1](https://www.linkedin.com/in/moe-kyaw-aung-2653093a1) |
| 🐙 GitHub | [Moekyawaung](https://github.com/Moekyawaung) |
| 🌐 Gravatar | [moekyawaung2026](https://gravatar.com/moekyawaung2026) |
| 🦋 Bluesky | [moekyawaung96.bsky.social](https://bsky.app/profile/moekyawaung96.bsky.social) |
| 📺 YouTube | [Channel](https://www.youtube.com/channel/UCdGC3lLlIPnb2VIL_qS65OQ) |
| 🎮 TikTok | [@moelay262411](https://tiktok.com/@moelay262411) |

</div>

---

## 📄 License

```
MIT License

Copyright (c) 2026 Moe Kyaw Aung

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.
```

See [LICENSE](LICENSE) for full text.

---

<div align="center">

Made with ❤️ in **Tachileik, Myanmar** · Portfolio V3 · 2026

[![Visitors](https://visitor-badge.laobi.icu/badge?page_id=Dev-moe-kyawaung.Moekyawaung-portfolios-V3)](https://github.com/Dev-moe-kyawaung/Moekyawaung-portfolios-V3)

</div>
