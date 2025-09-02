# AR Viewer — Minimal (GLB + USDZ)

A clean, single‑page AR viewer for **GitHub Pages**. No inputs, just a big viewer, one **Open in AR** button, and a QR code.

## Use
1. Put your files in `assets/` as:
   - `model.glb` (Android/Web & Scene Viewer)
   - `model.usdz` (iOS Quick Look)
2. Deploy on GitHub Pages (Settings → Pages → Deploy from a branch).
3. Share the page URL or QR. On phones, tap **Open in AR**.

If iOS doesn’t trigger from the button, there’s a fallback **Open on iOS** link using `<a rel="ar">` to open the USDZ directly in Quick Look.
