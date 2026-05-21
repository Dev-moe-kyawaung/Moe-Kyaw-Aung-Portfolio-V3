# 🚀 Deployment Guide

This portfolio is a **static single-file site** — it can be deployed anywhere static files are served.

---

## Option 1: GitHub Pages (Auto-Deploy) ⭐ Recommended

The repo includes a pre-configured GitHub Actions workflow (`.github/workflows/deploy.yml`) that automatically deploys on every push to `main`.

### Setup (one-time)

1. Go to your repo on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Build and deployment**, set **Source** to **GitHub Actions**
4. Save

### How it works

Every `git push` to `main` triggers:
```
Build → Validate → Upload artifact → Deploy to Pages
```

### Live URL

```
https://dev-moe-kyawaung.github.io/Moekyawaung-portfolios-V3/
```

---

## Option 2: Netlify (Drag & Drop)

1. Go to [netlify.com](https://netlify.com) and log in
2. Drag the project folder onto the Netlify dashboard
3. Done — Netlify gives you a URL instantly

**Or connect via Git:**
1. New site → Import from GitHub
2. Select `Moekyawaung-portfolios-V3`
3. Build command: *(leave empty)*
4. Publish directory: `/` (root)
5. Deploy

---

## Option 3: Vercel

```bash
# Install Vercel CLI
npm i -g vercel

# In the project folder
vercel deploy

# Follow prompts — select "other" for framework
```

---

## Option 4: Manual Upload (Any Host)

Upload `index.html` to any web host's public directory:
- cPanel File Manager → `public_html/`
- FTP client → server root
- Amazon S3 → public bucket with static hosting enabled

---

## Custom Domain

After deploying to GitHub Pages:

1. Go to **Settings → Pages → Custom domain**
2. Enter your domain (e.g. `moekyawaung.dev`)
3. Add a CNAME record at your DNS provider pointing to:
   ```
   dev-moe-kyawaung.github.io
   ```
4. Check "Enforce HTTPS" once DNS propagates

---

## Local Preview

```bash
# Clone
git clone https://github.com/Dev-moe-kyawaung/Moekyawaung-portfolios-V3.git
cd Moekyawaung-portfolios-V3

# Python server
python -m http.server 8080

# Visit
open http://localhost:8080
```

Or just double-click `index.html` — it works offline too.
