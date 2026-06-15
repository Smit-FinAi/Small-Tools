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
