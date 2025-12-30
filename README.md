# parcri.net

Personal site for Jared Lewis - Deterministic AI Architecture.

## Quick Deploy to GitHub Pages

### Option 1: New Repository

1. Create a new repository on GitHub named `parcri.net` (or any name)
2. Upload all files from this folder to the repository
3. Go to Settings → Pages
4. Under "Source", select "Deploy from a branch"
5. Select `main` branch and `/ (root)` folder
6. Click Save

Your site will be live at `https://yourusername.github.io/parcri.net/`

### Option 2: Using Git

```bash
# Initialize and push
cd parcri-deploy
git init
git add .
git commit -m "Initial deploy"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/parcri.net.git
git push -u origin main
```

Then enable Pages in repository settings.

## Custom Domain Setup (parcri.net)

### DNS Configuration

Add these records at your domain registrar:

| Type  | Name | Value                        |
|-------|------|------------------------------|
| A     | @    | 185.199.108.153              |
| A     | @    | 185.199.109.153              |
| A     | @    | 185.199.110.153              |
| A     | @    | 185.199.111.153              |
| CNAME | www  | yourusername.github.io       |

### GitHub Pages Settings

1. Go to Settings → Pages
2. Under "Custom domain", enter `parcri.net`
3. Check "Enforce HTTPS" (may take up to 24 hours)

The CNAME file in this repo is already configured for `parcri.net`.

## Files

- `index.html` - Main site
- `404.html` - Custom 404 page
- `favicon.svg` - Site icon
- `CNAME` - Custom domain configuration

## Tech

- Pure HTML/CSS (no build step)
- Dark mode via `prefers-color-scheme`
- NeXTSTEP-inspired design with Apple refinement
- Mobile responsive

---

© 2025 Jared Lewis · Houston
