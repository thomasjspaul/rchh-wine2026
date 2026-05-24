# wine.rchh.ca — NS Rotary Wine Fundraiser 2026

Landing page for the Harvest Wines & Spirits × Rotary Nova Scotia summer fundraiser.

## Adding Logos

Open `index.html` and find the two `<img>` tags marked with `LOGO:` comments.

1. Save your Rotary logo as `rotary-logo.png` in this folder, then set `src="rotary-logo.png"` on the first img.
2. Save the Harvest Wines logo as `harvest-logo.png`, then set `src="harvest-logo.png"` on the second img.

The page will automatically show the logo and hide the text placeholder once the file loads.

## Deploying to Cloudflare Pages

### 1. Create a GitHub repo

```
git init
git add index.html README.md
git commit -m "Initial fundraiser page"
git remote add origin https://github.com/YOUR_USERNAME/rchh-wine2026.git
git push -u origin main
```

### 2. Connect to Cloudflare Pages

1. Log in to [dash.cloudflare.com](https://dash.cloudflare.com) → **Pages** → **Create a project**
2. Choose **Connect to Git** → select your new repo
3. Build settings:
   - **Framework preset:** None
   - **Build command:** *(leave blank)*
   - **Build output directory:** `/`
4. Click **Save and Deploy**

### 3. Add the custom domain

1. In Cloudflare Pages → your project → **Custom Domains** → **Set up a custom domain**
2. Enter `wine.rchh.ca`
3. Since rchh.ca is already managed in Cloudflare, the CNAME record will be created automatically.

The page will be live at `https://wine.rchh.ca` within a few minutes.

## Making Updates

Edit `index.html`, commit, and push — Cloudflare Pages redeploys automatically within ~30 seconds.
