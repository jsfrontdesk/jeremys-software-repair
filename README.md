# Jeremy's Software Repair — website

Plain static site (HTML/CSS, no build step).

## Publish on GitHub Pages
1. Create a new public repo on GitHub (e.g. `software-repair`).
2. In this folder: `git remote add origin https://github.com/<you>/software-repair.git && git push -u origin main`
3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / `(root)`** → Save.
4. After ~1 minute the site is live at `https://<you>.github.io/software-repair/`.

## Custom domain (optional)
1. Buy a domain (e.g. from Namecheap, Cloudflare, Porkbun).
2. GitHub **Settings → Pages → Custom domain** → enter it (this adds a `CNAME` file).
3. At your DNS provider: for `www`, add a CNAME to `<you>.github.io`; for the root domain, add A records to 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153.
4. Once DNS resolves, tick **Enforce HTTPS**.
5. Add the final URL to `og:url` / JSON-LD `url` in `index.html` and a `Sitemap:` line in `robots.txt`.

## Edit
Prices and text are in `index.html`; colors in `style.css`.
