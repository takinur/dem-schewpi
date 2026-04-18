# dem-schewpi

A lightning-fast, design-forward landing page for **Dreams Event Management Ltd** — built with **Tailwind CSS** and **Alpine.js**, and deployed to the edge on **Vercel** for absurdly quick load times.

> Think “boutique agency website”, but engineered like it’s serving a million users (because why not).

**Live demo:** https://dem-schewpi.vercel.app

---

## What is this?

`dem-schewpi` is a clean, responsive, single-page marketing site focused on conversion:
- a crisp hero section with CTA
- service highlights (weddings, private celebrations, corporate events)
- a narrative “What we do?” section
- a contact/footer section

It’s intentionally simple: **one HTML file + Tailwind styles + assets** — easy to host, easy to edit, hard to break.

---

## Tech stack

- **HTML5** (single page)
- **Tailwind CSS** (utility-first styling)
- **Alpine.js** (tiny interactivity, e.g. mobile nav toggle)
- **Feather Icons** (icons via CDN)
- **Google Fonts (Poppins)**

---

## Project structure

```text
.
├── index.html
├── assets/
│   ├── css/
│   │   └── tailwind.css
│   └── image/
│       └── *.svg
└── LICENSE
```

---

## Getting started (local)

### 1) Clone
```bash
git clone https://github.com/takinur/dem-schewpi.git
cd dem-schewpi
```

### 2) Run locally
Since this is a static site, you can open `index.html` directly, but using a local server is better.

**Option A: VS Code Live Server**
- Install “Live Server”
- Right click `index.html` → “Open with Live Server”

**Option B: Python**
```bash
python -m http.server 5173
```
Then open:
- http://localhost:5173

---

## Customization guide

### Update branding
- Navbar logo: `assets/image/navbar-logo.svg`
- Footer logo: `assets/image/footer-logo.svg`

### Update hero text
Edit `index.html`:
- `<title>Dreams Event Management Ltd</title>`
- Hero headline and description text in the `<header>` section.

### Update contact info
Edit the footer section in `index.html` (look for `id="contact"`).

---

## Deployment

This project is ideal for:
- **Vercel**
- **Netlify**
- **GitHub Pages** (if you later enable Pages)

For Vercel: import the repo and deploy as a static site (no build step required unless you introduce a Tailwind build pipeline).

---

## Roadmap (high-impact upgrades)

If you want to turn this into a “serious” production-grade site:

- Add proper **SEO** (OpenGraph/Twitter meta, canonical URL, sitemap)
- Add a real **contact form** (Formspree/Resend/serverless function)
- Replace CDN assets with pinned/hashed assets for stricter **CSP**
- Add Tailwind build step (PostCSS) to generate a **tiny production CSS**
- Add **Lighthouse** + CI checks to keep performance “unfairly good”

---

## License

Licensed under the **Apache License 2.0**. See `LICENSE` for details.

---

## Credits

Built and maintained by **@takinur**.  
If you use this as a template, a star is appreciated (and legally binding in spirit).