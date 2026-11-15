# AKV BG

Free background remover for images. It runs fully in your browser, so your photos are never uploaded to any server.

இலவச Image Background Remover. உங்கள் photo உங்கள் browser-லேயே process ஆகும், எங்கும் upload ஆகாது.

**Live site:** https://your-site-link-here

## Features

- Removes the background with AI, right on your device
- No sign-up, no credits, no upload
- Tamil and English interface (தமிழ் / English)
- Preview original and result side by side
- Choose a transparent, white, yellow, blue or dark background
- Download the result as a PNG
- Works on phones and desktops

## How it works

1. Choose a photo (JPG, PNG or WebP).
2. The AI model downloads once on first use (about 40 MB) and is then cached by the browser.
3. The background is removed on your device.
4. Pick a background color and download the PNG.

## Project files

```
index.html   The whole site: HTML, CSS and JavaScript in one file
README.md    This file
```

## Deploy

The site is a single static file, so any static host works.

**Netlify:** open app.netlify.com/drop and upload a zip that contains `index.html` at its top level.

**Cloudflare Pages:** Workers & Pages → Create → Pages → Direct Upload → upload the zip.

**GitHub Pages:** push this repo, then go to Settings → Pages → Branch: `main` / root → Save.

Open the deployed link in Chrome to test it. Some in-app preview browsers cannot run the AI model or download files.

## Built with

- HTML, CSS and JavaScript (no build step)
- [@imgly/background-removal](https://github.com/imgly/background-removal-js) for in-browser background removal
- Baloo Thambi 2 font from Google Fonts

## License note

`@imgly/background-removal` is released under the AGPL-3.0 license, with a separate commercial license available from IMG.LY. Check their terms before using this project for a commercial service.

## Troubleshooting

- **Stuck on "Loading AI model":** check your internet connection and try again. The first load needs to download the model.
- **Download does not work:** open the site in Chrome instead of an in-app browser.
- **Slow on big photos:** resize the photo to about 2000 px or less and try again.
