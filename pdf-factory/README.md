# The PDF Factory — by Smit Parekh

A 40-tool PDF toolkit that runs 100% in the browser (merge, split, compress,
convert, sign, watermark, OCR, and more). No server, no uploads — and now
installable as a PWA on phone, PC and Mac.

## 📁 Files

```
index.html          ← the app (was pdf-factory.html)
manifest.json       ← PWA manifest (name, icons, colors)
sw.js               ← service worker (offline caching)
icons/              ← app icons (192/512, maskable, favicon, apple-touch-icon)
```

Keep all of these in the **same folder**, at the **root** of the repo (or in
`/docs` if you configure Pages that way) — the paths inside `index.html`,
`manifest.json` and `sw.js` are all relative.

## 🚀 Deploy to GitHub Pages

1. Create a new GitHub repo (e.g. `pdf-factory`) and upload all the files
   above, keeping the `icons/` folder structure intact.
2. In the repo: **Settings → Pages → Build and deployment → Source** → select
   **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
3. Wait ~1 minute, then open the URL GitHub gives you, e.g.
   `https://yourusername.github.io/pdf-factory/`.

PWAs require HTTPS — GitHub Pages already serves over HTTPS, so you're good.

## 📲 Install on your phone

**Android (Chrome):** open the site → tap the **⋮** menu → **"Install app"**
(or **"Add to Home screen"**). You can also tap the **Install App** button
that appears in the header. It then opens in its own window with no browser
bar, like a normal app.

**iPhone/iPad (Safari):** open the site → tap the **Share** icon → **"Add to
Home Screen"**.

## 💻 Install on PC / Mac (Chrome, Edge, Brave)

Open the site → click the **install icon** in the address bar (or the
**Install App** button in the header) → **Install**. It will appear as a
desktop app with its own shortcut, taskbar/dock icon, and window.

## 🔄 Offline use

After the first visit, the service worker caches the app and the libraries
it depends on (pdf-lib, pdf.js, JSZip, FileSaver, Roboto font). Subsequent
visits — including fully offline ones — will load from cache.

If you edit `index.html` later and the changes don't show up after
re-deploying, bump the `CACHE_NAME` value at the top of `sw.js` (e.g.
`pdf-factory-v1` → `pdf-factory-v2`) so the service worker installs a fresh
cache.
