# Randall Ricketts Design — Website Clone

A clean, static HTML/CSS/JS clone of [randallrickettsdesign.com](http://www.randallrickettsdesign.com), redesigned with an artisan aesthetic.

## Pages

| File | Page |
|------|------|
| `index.html` | Home |
| `gallery.html` | Gallery (with lightbox) |
| `options.html` | Stool heights |
| `woods.html` | Wood varieties (with lightbox) |
| `about.html` | About Randall |
| `schedule.html` | Show schedule |
| `contact.html` | Contact form |

## Local development

No build step needed — open any `.html` file directly, or use a local server:

```bash
# Python 3
python -m http.server 8000

# Node (npx)
npx serve .
```

Then visit `http://localhost:8000`.

## Deploy to Vercel

### Option A — Vercel CLI

```bash
npm i -g vercel
vercel
```

Follow the prompts. Vercel auto-detects the static site.

### Option B — GitHub + Vercel Dashboard

1. Push this folder to a GitHub repo.
2. Go to [vercel.com](https://vercel.com) → **Add New Project**.
3. Import your GitHub repo.
4. Leave all settings as defaults (Framework: **Other**, output: root).
5. Click **Deploy**.

That's it — the `vercel.json` handles clean URLs and cache headers.

## Notes

- Images are loaded directly from the original site's CDN (`randallrickettsdesign.com`). If you want a fully self-contained site, download the images and update the `src` paths.
- The contact form is a front-end-only demo. To make it functional, connect it to a service like [Formspree](https://formspree.io) or [Netlify Forms](https://www.netlify.com/products/forms/).
- Fonts load from Google Fonts (Cormorant Garamond + Josefin Sans).
