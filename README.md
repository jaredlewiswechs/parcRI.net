# parcri.net

Personal site for Jared Lewis - Deterministic AI Architecture.

## Automated Deployment

This repository is configured for automatic deployment to GitHub Pages via GitHub Actions.

### Setup

1. Go to repository Settings → Pages
2. Under "Source", select **GitHub Actions**
3. Push to the `main` branch to trigger deployment

The site will automatically deploy on every push to `main`. The workflow can also be triggered manually from the Actions tab.

### First-Time Setup

If this is a new repository:

1. Push your code to the `main` branch
2. Enable GitHub Pages in Settings → Pages
3. Select "GitHub Actions" as the source
4. The deployment workflow will run automatically

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
