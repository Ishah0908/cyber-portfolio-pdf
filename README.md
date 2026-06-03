# Cyber Portfolio PDF Edition

Static portfolio for Ibrahim Sultan using a hacker HUD aesthetic and PDF cards.

## Public Blog Routes

- Blog home: `/blog/`
- Starter posts:
	- `/blog/posts/sase-ztna-field-notes`
	- `/blog/posts/iam-pam-breakglass`

Add or edit blog files in `blog/` to publish more posts under your same domain.

## 1) Add your PDFs

- Put all final PDFs inside the `pdfs/` folder.
- Update the `docs` array in `index.html` to match your final filenames and titles.

## 2) Edit Blog Content

- Update `blog/index.html` to change post cards.
- Create new posts inside `blog/posts/` as `.html` files.
- Link each new post from `blog/index.html`.

## 3) Local Preview

Open `index.html` directly in your browser, or run a static server:

```bash
cd cyber-portfolio-pdf
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## 4) GitHub -> Vercel (Free)

```bash
cd ~/cyber-portfolio-pdf
git init
git add .
git commit -m "Initial PDF portfolio scaffold"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

In Vercel:

1. New Project
2. Import the GitHub repo
3. Framework preset: Other
4. Deploy

Every push to `main` auto-deploys.

## 5) Free Fallback Hosting

- Cloudflare Pages: connect same GitHub repo, build command empty, output `/`.
- GitHub Pages: works for static hosting, but Vercel is cleaner for custom domains and previews.

## Notes

- Keep file names URL-safe, for example `sase-ztna-blueprint.pdf`.
- If files are very large, use compressed PDFs to keep repo size reasonable.
