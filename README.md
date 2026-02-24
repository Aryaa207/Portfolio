# Aryaa Vijay — Portfolio

Professional aerospace engineering portfolio built from scratch.

## File Structure

```
portfolio/
├── index.html          ← Your entire site (edit this)
└── assets/
    ├── drone.glb       ← Hero 3D model (your drone)
    ├── missile.stl     ← Hypersonic missile model
    └── sr71.stl        ← SR-71 Blackbird model
```

## Deploy to GitHub Pages (30 minutes)

### Step 1 — Create GitHub repo
1. Go to github.com → New repository
2. Name it exactly: `portfolio` (or your GitHub username if you want `username.github.io`)
3. Set to **Public**
4. Don't add README (you have one)

### Step 2 — Upload files
1. Click "Upload files" in the repo
2. Upload `index.html`
3. Create folder `assets/` and upload:
   - `drone.glb`
   - `missile.stl`
   - `sr71.stl`

### Step 3 — Enable GitHub Pages
1. Go to repo **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / `root`
4. Click Save
5. Your site will be live at `https://yourusername.github.io/portfolio` in ~2 minutes

### Step 4 — Point your domain (aryaavijaysportfolio.com)
In GitHub Pages settings, add your custom domain: `aryaavijaysportfolio.com`

Then in your domain registrar (wherever you bought the domain), add these DNS records:
```
A     @    185.199.108.153
A     @    185.199.109.153
A     @    185.199.110.153
A     @    185.199.111.153
CNAME www  yourusername.github.io
```

Wait 10–30 minutes for DNS to propagate. Done.

## Customization

All content is in `index.html`. Search for these to update:
- `Aryaa Vijay` — your name
- `avijay2024@my.fit.edu` — your email
- `+1 (425) 738-9190` — your phone
- Project links point back to your Squarespace portfolio pages (already set)
- Update LinkedIn URL: find `linkedin.com/in/yourprofile` and replace

## Adding More 3D Models

Drop `.stl` or `.glb` files in `assets/` and add a new canvas + `makeSTLScene()` call in the script.
