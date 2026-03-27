# STAMM — Baumpatenschaften im Berner Oberland

Tree sponsorship website. Static site hosted on GitHub Pages.

## Structure

```
├── index.html          # Main landing page (DE/EN bilingual)
├── impressum.html      # Legal notice (required in CH)
├── CNAME               # Custom domain config
└── assets/
    ├── logos/          # SVG + PNG logo files
    └── images/         # Forest photos (add your own)
```

## Setup

1. Push to GitHub
2. Enable GitHub Pages (Settings → Pages → Source: main branch)
3. Add custom domain: `stamm-wald.ch`
4. Configure DNS at your registrar:
   - A records pointing to GitHub Pages IPs
   - CNAME record: `www` → `<username>.github.io`

## Adding Photos

Drop your forest photos into `assets/images/` and update the `<img>` tags in `index.html`.

## Domain DNS Records

Add these at your domain registrar (GoDaddy):

```
Type    Name    Value
A       @       185.199.108.153
A       @       185.199.109.153
A       @       185.199.110.153
A       @       185.199.111.153
CNAME   www     <your-username>.github.io
```
