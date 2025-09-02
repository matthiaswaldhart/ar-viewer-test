# AR Viewer — GitHub Pages Starter

A tiny, free, app‑less AR viewer you can host on **GitHub Pages**. It uses Google’s `<model-viewer>` web component to display `.glb` (Android/Web) and `.usdz` (iOS Quick Look) with a built‑in **QR code** for easy sharing.

## What you get
- **index.html** — viewer page (reads `?src=` and `?ios-src=` query params)
- **assets/** — put your `model.glb` and `model.usdz` here (or host anywhere and use full URLs)
- Built‑in **QR code** that points to the exact URL (with params)

---

## Step 1 — Create a GitHub repo
1. Go to https://github.com/new
2. Name it, e.g. `ar-viewer`.
3. Click **Create repository**.

## Step 2 — Add these files
- Upload the contents of this folder to your repo (keep `assets/`).
- Put your `model.glb` and `model.usdz` files into `assets/` (or elsewhere).

## Step 3 — Enable GitHub Pages
1. In your repo, go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source = Deploy from a branch**.
3. Select branch **main** (or `master`) and folder **/ (root)**. Click **Save**.
4. Wait ~1 minute. You’ll get a URL like: `https://<username>.github.io/<repo>/`.

## Step 4 — Test it
Open: `https://<username>.github.io/<repo>/`

- Default paths:
  - GLB → `/assets/model.glb`
  - USDZ → `/assets/model.usdz`

Replace with your files or paste full URLs into the inputs, press **Apply**, then **Copy sharable URL**. The QR code updates automatically.

## Optional — Deep links for multiple models
You can generate links for each student/model using query params:
```
https://<username>.github.io/<repo>/?src=https://.../look1.glb&ios-src=https://.../look1.usdz
```
Print those as QR codes; scanning opens AR immediately on phones.

## Notes & tips
- iOS opens `.usdz` via **Quick Look**; Android uses **Scene Viewer** for `.glb`.
- Keep files reasonably small (optimize meshes, compress textures) for fast loading.
- Host large assets on GitHub Releases, Git LFS, or another CDN if needed.
- If AR doesn’t launch on desktop, try on a phone — AR is mobile‑first.

## Credits
- `<model-viewer>` (Google) — https://modelviewer.dev
- QRCode.js by Kazuhiko Arase
