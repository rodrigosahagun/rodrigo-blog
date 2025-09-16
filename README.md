# Rodrigo Blog — Static Site for Vercel + GitHub

This is a zero‑build static blog. Just push these files to a GitHub repo and import the project in Vercel.

## Files
- `index.html` — The entire site (list + post view) using hash routing.
- `posts.js` — Weekly posts database (edit this file to add new posts).
- `vercel.json` — SPA routing rewrite so all paths resolve to `index.html`.
- `assets/` — Put your images here (optional).

## Quick Start
1. **Create GitHub repo** (e.g., `rodrigo-blog`).
2. Add these files and commit.
3. Go to **vercel.com → Add New Project → Import GitHub Repo**.
4. Framework Preset: **Other** (since it's static). No build command. Output directory: `/`.
5. Click **Deploy**. Your site will be live at `https://<project>.vercel.app`.

## Adding a New Post (weekly)
- Open `posts.js` and duplicate the first object.
- Change `id`, `title`, `date`, `tags`, `cover`, `summary` and `content` (HTML).
- Commit to `main` — Vercel deploys automatically.

## Pretty URLs
This SPA uses hash routes (`#/post/:id`) so it works on static hosting.
If you later migrate to Next.js, you can switch to real URLs easily.

## Optional Custom Domain
- In Vercel → **Settings → Domains** → Add `rodrigosahagun.com` (or similar) and follow DNS steps.

## SEO Tips
- Keep `title` and `meta description` updated in `index.html`.
- Use descriptive `cover` images and `alt` attributes when you add images inline.

---
Built for Rodrigo by ChatGPT.
