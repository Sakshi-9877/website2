# Daily Notes — Minimal Daily Blog

This is a small, minimal, and professional static site for short daily blog entries.

Files
- `index.html` — main page and static content for the blog.
- `style.css` — site styles (responsive, minimal design).

Quick preview

1. Open the site directly by double-clicking `index.html` in your file explorer. That opens the page in your default browser.

2. Or serve the folder with a simple local HTTP server (recommended for correct asset handling):

PowerShell / Command Prompt

```powershell
cd website2
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

macOS / Linux

```bash
cd website2
python3 -m http.server 8000
# then open http://localhost:8000
```

Development notes
- The site is intentionally static so content can be edited directly in `index.html` for quick additions.
- To manage posts separately, consider adding a `posts.json` and a tiny script to fetch and render entries.

Suggested next steps
- Add a small JavaScript loader to pull posts from `posts.json`.
- Add an author/metadata section for each post to make it machine-readable (microformats or JSON-LD).
- Deploy to GitHub Pages or any static hosting (Netlify, Vercel) for easy publishing.

Deployment (GitHub Pages)

```bash
# from repository root
git add website2
git commit -m "Add static Daily Notes site"
git push origin main
# enable GitHub Pages for the branch in repo settings or use an actions workflow
```

License & author
- License: MIT (change as you prefer)
- Author: You — update this README with your name and contact info.

If you want, I can:
- Add a `posts.json` loader and simple JS to render posts dynamically.
- Wire up a GitHub Actions workflow to deploy to GitHub Pages.
