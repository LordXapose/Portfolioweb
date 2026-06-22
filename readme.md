<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:141D2B,100:9FEF00&height=160&section=header" />

# 🌐 Portfolio Kaushal Patidar

**A WebGL-powered creative portfolio with dual Security × Business personas**

[![HTML](https://img.shields.io/badge/HTML-Single_File-141D2B?style=flat-square&logo=html5&logoColor=9FEF00)](#)
[![Three.js](https://img.shields.io/badge/Three.js-r128-141D2B?style=flat-square&logo=threedotjs&logoColor=9FEF00)](#)
[![Zero Build](https://img.shields.io/badge/Zero_Build-No_Dependencies-141D2B?style=flat-square&logo=rocket&logoColor=9FEF00)](#)
[![Deploy](https://img.shields.io/badge/Deploy-GitHub_Pages-141D2B?style=flat-square&logo=github&logoColor=9FEF00)](#-deploy)

<br />

[**Live Demo →**](#) · [**LinkedIn →**](https://www.linkedin.com/in/kaushal-patidar-kenil4sec/) · [**GitHub →**](https://github.com/LordXapose)

</div>

---

## ✨ Features

### 🎨 Visual

- **WebGL shader hero** — GLSL fragment shader rendering real-time liquid noise, mouse-reactive, recolors by persona
- **Intro loader** — 0→100 counter with curtain-wipe reveal
- **Custom cursor** — lag-follow ring with sparkle trail (✦), magnetic hover on interactive elements
- **Film grain overlay** with SVG noise texture
- **Hack The Box palette** — `#141D2B` dark navy · `#9FEF00` neon green · `#00CCFF` electric cyan

### 🐾 Delight

- **Click-to-cycle mascot zoo** — parrot → cat → fox → owl → penguin, each with:
  - Cursor-following eyes + auto-blink
  - Gentle sway animation (ears/tuft)
  - Happy hop + confetti burst on click
  - Unique sound bubble on hover (*squawk! / meow! / yip! / hoot! / noot!*)
- **Confetti bursts** on mode-switch and email click
- **Decode/scramble effect** on scroll-highlight verbs

### 📄 Content Sections

| Section | Description |
|:--------|:------------|
| **Hero** | Full-viewport name + tagline over the WebGL shader |
| **"You can ___"** | Sticky scroll-highlight list — *design · prototype · break · secure · analyze · build · ship* |
| **About** | Compact circle avatar + persona-aware bio |
| **The Pivot** | Vertical timeline tracing the Security → Finance career journey |
| **Experience** | Role cards with period, title, and organization |
| **Projects** | 3-column card grid with glassmorphism, hover glow, and tag chips |
| **Skills** | Grouped chips — Offensive, Defensive, Finance categories |
| **Education** | Credential rows with accent-colored dates |
| **Contact** | Dark footer — "Let's talk." heading + accent-underlined email + social links |

### 🔀 Dual Persona Toggle

Switch between **Security** and **Business** mode — from the nav or by pressing `t`:

| | Security | Business |
|:--|:---------|:---------|
| **Accent** | `#9FEF00` neon green | `#00CCFF` cyan |
| **Shader** | Green-dominant liquid field | Cyan-dominant liquid field |
| **Content** | Offensive security, red team, CTF | Strategy consulting, IB, FinTech |
| **Projects** | XSS Scanner, C2 Server, Malware Sandbox | PlotPilot, Secure Storage, DeFi research |
| **Skills** | OWASP, Recon, Malware Analysis | Financial Engineering, PE, Consulting |

---

## 🛠 Tech Stack

```
HTML          Single self-contained file, zero build step
Three.js      r128 (CDN) — WebGL fragment shader
GLSL          Custom fbm noise with mouse uniform + persona lerp
CSS           CSS variables, clamp(), color-mix(), backdrop-filter
JS            Vanilla — IntersectionObserver, Web Animations API, requestAnimationFrame
Fonts         Bricolage Grotesque + Hanken Grotesk + JetBrains Mono (Google Fonts CDN)
```

No frameworks. No bundler. No `node_modules`. Open the file in a browser and it works.

---

## 🚀 Deploy

### GitHub Pages (free, 5 minutes)

```bash
# 1. Clone or create a repo
git init my-portfolio && cd my-portfolio

# 2. Rename the file
mv creative.html index.html

# 3. Push to GitHub
git add . && git commit -m "initial portfolio"
git remote add origin https://github.com/LordXapose/LordXapose.github.io.git
git branch -M main && git push -u origin main
```

4. Go to **Settings → Pages → Source: main / root → Save**
5. Your site is live at `https://lordxapose.github.io` in ~60 seconds

### Any static host

It's a single HTML file — drag and drop to Netlify, Vercel, Cloudflare Pages, or any web server.

---

## 📁 Project Structure

```
.
├── index.html          # The entire portfolio (single file)
├── README.md           # This file
├── og-image.png        # Social share card (1200×630)
├── manifest.webmanifest
├── robots.txt
├── sitemap.xml
└── .nojekyll           # Prevents Jekyll from processing on GitHub Pages
```

---

## 🎯 Customization

All content lives in a `<script>` data block at the top of the HTML file:

```javascript
const COMMON = { name, email, socials, education, journey, ... };
const MODES = {
  cyber:    { tagline, about, projects, skills, experience, ... },
  business: { tagline, about, projects, skills, experience, ... },
};
```

Edit the data objects → save → refresh. No build step needed.

---

## ⚡ Performance Notes

- The WebGL shader is GPU-accelerated and runs at 60fps on modern hardware
- `prefers-reduced-motion` is fully respected — all animations, transitions, and the cursor trail are disabled
- Touch devices get native cursors (no custom cursor overhead)
- The headshot is embedded as base64 to keep it zero-dependency
- Three.js loads from CDN with a static gradient fallback if blocked

<div align="center">

<sub>Cybersecurity × Finance · Leipzig, DE</sub>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:141D2B,100:9FEF00&height=100&section=footer" />

</div>
