# Hosting guide

This project is a static website.

## Recommended document root
Point your web server document root to:

`matata-tours--master/Tour/`

This ensures all relative links like `assets/...` and `*.html` work directly.

## If your server uses repository root as document root
A root-level `index.html` redirect is included and will forward visitors to:

`matata-tours--master/Tour/index.html`

## Quick local test
From repository root:

```bash
python3 -m http.server 8000
```

Then open:
- `http://localhost:8000/` (redirects to site)
- `http://localhost:8000/matata-tours--master/Tour/index.html`
