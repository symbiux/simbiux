# Symbiux website

Static HTML/CSS/JS site. No build step, no backend. All asset paths are relative, so it also works under a repo subpath.

## Update
Edit `index.html` (CSS and JS are inline). Push to `main`; the workflow redeploys.

## Contact form
Set `FS` in the script at the bottom of `index.html` to your Formspree endpoint. If empty, the form opens a prefilled email (mailto fallback).

## Deploy
1. Create a GitHub repo and push these files to `main`.
2. Settings > Pages > Source: **GitHub Actions**.
3. `CNAME` already contains `symbiux.com`.
4. At your domain provider add A records for `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153, and a CNAME for `www` pointing to `<username>.github.io`.
5. After DNS verifies, tick **Enforce HTTPS** in Settings > Pages.

## Still to do
- Add `og.png` (1200x630) for social sharing.
- Domain and deployment are not configured until you complete the steps above.
