# JAYS TO SPLIT

Single-file training site. Everything is embedded in `index.html` — all photos, all styles, all code. Nothing to build, nothing to install.

## Put it live on GitHub Pages

1. Go to **github.com/new**. Name the repo whatever you want. Set it to **Public**. Create it.
2. On the empty repo page, click **uploading an existing file**.
3. Drag in these three files:
   - `index.html` — required
   - `apple-touch-icon.png` — optional, the icon when you save it to your home screen
   - `og.png` — optional, the image that shows when you text someone the link
4. Click **Commit changes**.
5. Go to **Settings → Pages**. Under *Build and deployment*, set **Source: Deploy from a branch**, **Branch: main**, **Folder: / (root)**. Save.
6. Wait about a minute, then refresh. Your URL appears at the top of that page:
   `https://YOUR-USERNAME.github.io/YOUR-REPO/`

That's it. Any time you want to change something, upload a new `index.html` over the old one and it goes live in under a minute.

### Want it at `yourname.github.io` with no `/repo` on the end?

Name the repository exactly `YOUR-USERNAME.github.io`. Same steps otherwise.

## On your phone

Open the URL in Safari → Share → **Add to Home Screen**. It launches full screen with no browser bars, like an app.

## Link previews

If you want the preview image to show when you send the link in Messages or post it anywhere, open `index.html`, find these two lines near the top:

```html
<meta property="og:image" content="og.png">
<meta name="twitter:image" content="og.png">
```

Replace `og.png` in both with your full URL, e.g.:

```html
<meta property="og:image" content="https://YOUR-USERNAME.github.io/YOUR-REPO/og.png">
```

Relative paths work in some apps but not all. The full URL always works.

## Your data

Every PR and set you log is saved in your browser on that device only. It is not uploaded anywhere and nobody else can see it, even though the page is public.

This means: log on your phone, and your phone holds the data. If you open the site on a laptop it starts empty. Use **PRs → history → export** to save a backup file, and **import** to load it on another device or after clearing your browser.

## Custom domain (optional)

If you own a domain, add it under **Settings → Pages → Custom domain**. GitHub will walk you through the DNS records.
