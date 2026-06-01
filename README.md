# ClarezAI Website

A fast, responsive, multi-page marketing site for **ClarezAI** — *Precision Strategic Intelligence for Medical Affairs*.

Built as plain HTML/CSS/JS — **no build step, no dependencies**. Open the files directly or upload them to any static web host.

## Pages

| File | Page |
|------|------|
| `index.html` | Home — hero, the engine overview, capabilities, value drivers, business impact |
| `solution.html` | Solution — the Central Intelligence Engine, 5 modules, lifecycle, value drivers |
| `about.html` | About — Why ClarezAI, credentials, differentiation |
| `contact.html` | Contact — details + JotForm placeholder |

## Project structure

```
ClarezAI-website/
├── index.html
├── solution.html
├── about.html
├── contact.html
└── assets/
    ├── css/styles.css      ← design system (brand colors, components, responsive)
    ├── js/main.js          ← sticky header, mobile menu, scroll reveal
    └── img/
        ├── clarezai-logo.png        ← header logo
        ├── clarezai-logo-white.png  ← footer logo (white variant)
        ├── clarezai-mark.png        ← eye/network icon only
        └── favicon.png
```

## Preview locally

Double-click `index.html`, or run a tiny local server (recommended so paths resolve cleanly):

```powershell
python -m http.server 8000
# then open http://localhost:8000
```

## Connect the contact form (JotForm)

Open `contact.html` and find the block marked `JOTFORM EMBED` (the `<div class="contact-embed">`).
Replace the `<div class="embed-placeholder">…</div>` with your JotForm **iframe** embed code, e.g.:

```html
<iframe title="ClarezAI contact form"
  src="https://form.jotform.com/YOUR_FORM_ID"
  allowtransparency="true" scrolling="no"
  style="width:100%;min-height:560px;border:none;"></iframe>
```

(Or keep a simple button that links to your hosted form.)

## Update contact email

The placeholder address `info@clarezai.com` appears in every footer and on the contact page —
search & replace it with your real address.

## Brand (in `assets/css/styles.css` → `:root`)

- Gradient: Cyan `#28BEEC` → Blue `#0E5BC4` → Deep blue `#0B3E8C`
- Ink `#15212E`, Slate `#51657A`, Navy `#0A2540`
- Fonts: **Sora** (headings) + **Inter** (body), via Google Fonts

## Deploy

Upload the whole folder to any static host — **Netlify, Vercel, GitHub Pages, Cloudflare Pages**,
or any standard web host. No configuration required.
