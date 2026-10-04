# Unmanned Systems Lab — website

Static site. No build step, no dependencies. Edit the HTML and push.

## Publish on GitHub Pages

1. Create a public repo named `usl-site` (any name works) under your GitHub account.
2. Upload every file in this folder to the repo root, including the hidden `.nojekyll`.
3. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main`, folder: `/ (root)` → Save.
4. In about a minute the site is live at `https://<your-username>.github.io/usl-site/`.

## Custom domain (optional, ~$12/year)

1. Buy a domain (Namecheap, Cloudflare Registrar, Porkbun).
2. At the registrar, add these DNS records:
   - Four `A` records for the apex (`@`): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One `CNAME` for `www` → `<your-username>.github.io`
3. Settings → Pages → Custom domain: enter the domain, Save, then tick **Enforce HTTPS**.

## Files

- `index.html` — home
- `research.html` — research directions, facilities
- `publications.html` — books, journals, conferences
- `people.html` — current members, alumni
- `news.html` — full news list
- `join.html` — recruiting
- `style.css` — all styling, including light and dark themes

## How students update it

Have them fork the repo, edit the relevant HTML, and open a pull request.
The news items, people, and publications are plain HTML blocks — copy an
existing one and change the text.

Items marked with a dashed orange box are placeholders that still need content.
Search for `class="todo"` to find them all, and delete the box when filled.
