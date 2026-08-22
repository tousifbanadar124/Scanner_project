# ScanForge — QR Code Generator

A fast, private, client-side QR code generator. Build codes for links, text,
Wi-Fi, email, phone numbers, and contact cards, then export as PNG or SVG.
Everything runs in the browser — no backend, no data collection.

## 🚀 Deploy this on GitHub Pages (free hosting)

**1. Create a new repository**
- Go to [github.com/new](https://github.com/new)
- Name it anything, e.g. `scanforge` or `qr-generator`
- Keep it **Public** (required for free GitHub Pages)
- Click **Create repository**

**2. Upload the file**
- On your new repo's page, click **Add file → Upload files**
- Drag in `index.html` from this folder
- Scroll down, click **Commit changes**

> The file must be named exactly `index.html` and sit in the root of the
> repo (not inside a subfolder) — this is what's included here.

**3. Turn on GitHub Pages**
- In your repo, go to **Settings → Pages** (left sidebar)
- Under "Build and deployment" → **Source**, choose **Deploy from a branch**
- Under **Branch**, choose `main` and folder `/ (root)`, then **Save**

**4. Visit your live site**
- After ~1 minute, GitHub shows a URL at the top of the Pages settings, e.g.:
  `https://your-username.github.io/scanforge/`
- Open it — your QR generator is live.

Any time you want to update the site, edit `index.html` and commit again
(or upload a new version) — GitHub Pages redeploys automatically within a
minute or two.

## Alternative: deploy with Git from your computer

```bash
git init
git add index.html README.md
git commit -m "Initial commit: ScanForge QR generator"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
git push -u origin main
```

Then enable Pages as described in step 3 above.

## Notes on how it works

- The QR engine (`qrcode-generator`) and fonts (Google Fonts) load from
  public CDNs over HTTPS — this works fine on GitHub Pages with no extra
  configuration.
- No build step, no `npm install`, no server — it's a single static HTML
  file, which is exactly what GitHub Pages serves best.
- If you ever want a custom domain, add a `CNAME` file with your domain name
  in the repo root and point your DNS to GitHub Pages (see GitHub's docs for
  exact records).

## File structure

```
your-repo/
├── index.html   ← the whole site (HTML + CSS + JS)
└── README.md    ← this file
```
