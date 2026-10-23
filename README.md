# Muhammad Zair Ali — Portfolio

A single self-contained `index.html` (HTML + CSS + JS all in one file) with a
two-tab layout (Design / Video Editing). Ready for GitHub Pages — no build step.

## Folder structure

```
portfolio/
├── index.html
└── assets/
    └── design/
        ├── brand-identity/
        ├── logos/
        ├── social-media-posts/
        ├── carousel-posts/
        ├── presentation/
        ├── reports/
        └── miscellaneous/
```

## Adding a design project

1. Export/download the image (JPG, ~1200–1400px wide is plenty — don't upload huge files).
2. Drop it into the matching folder, e.g. `assets/design/logos/project-14.jpg`.
3. In `index.html`, find that category's grid (search for `id="logos"`, etc.) and
   duplicate a `<figure class="card">...</figure>` block, then update:
   - the `src` path
   - the `alt` text
   - the title and description inside `<figcaption>`

## Adding a video project

1. Upload the video to YouTube as **Unlisted** (Visibility → Unlisted when publishing).
2. Open the video, click Share → Embed, and copy the video ID from the URL (the
   part after `/embed/` or after `v=` on a normal link).
3. In the Video panel of `index.html`, duplicate a `<figure class="card video-card">`
   block and replace `VIDEO_ID` in the iframe `src` with your real ID.

## Deploying to GitHub Pages

1. Create a new repo on GitHub (e.g. `portfolio`).
2. Push this folder's contents to the repo root:
   ```
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
   git push -u origin main
   ```
3. On GitHub: Settings → Pages → Source → select `main` branch, `/ (root)` folder → Save.
4. Your site will be live at `https://YOUR_USERNAME.github.io/portfolio/` within a minute or two.

## Before going live

- [ ] Fill in the remaining categories with your real projects
- [ ] Replace `youremail@example.com` and social links in the Contact section
- [ ] Remove any empty/placeholder cards you haven't filled in yet
- [ ] Swap in your real video embeds once uploaded to YouTube
