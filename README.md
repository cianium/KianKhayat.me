# kiankhayat.me

Personal portfolio of **Kian Khayat** (کیان خیاط): AI enthusiast, Python developer and future software engineer.

**Live:** https://kiankhayat.me

## Features

- Single-page site in pure HTML, CSS and JavaScript. No framework, no build step.
- Light and dark themes with a persistent toggle.
- Skills as story-style bubbles, project cards, certificate timeline and articles.
- Live GitHub contribution heatmap.
- Contact form powered by EmailJS.
- SEO: canonical URL, Open Graph and Twitter cards, JSON-LD (`WebSite` and `Person`, including the Persian name), `sitemap.xml` and `robots.txt`.
- Accessibility: semantic landmarks, ARIA labels, keyboard-friendly modals and cards.

## Project structure

```
.
├── index.html            # the whole site (markup, styles, scripts, content data)
├── favicon.svg           # logo, navy rounded square (source of all icons)
├── favicon.ico
├── favicon-48x48.png
├── favicon-96x96.png
├── icon-192.png
├── icon-512.png
├── apple-touch-icon.png
├── logo-mark.svg         # transparent gold "K" for use on dark backgrounds
├── site.webmanifest
├── photo.jpg             # 800×800 portrait used for Open Graph and structured data
├── 123.png               # hero portrait
├── robots.txt
├── sitemap.xml
└── CNAME                 # custom domain for GitHub Pages
```

## Editing content

Skills, projects, articles and certificates live in the `SKILLS`, `PROJECTS`, `ARTICLES` and `CERTS` arrays at the top of the `<script>` block in `index.html`. Add an object to an array and the page renders it.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deployment

Hosted on GitHub Pages from the `main` branch. The `CNAME` file binds the site to `kiankhayat.me`. Every push to `main` goes live within a minute or two.

## After changing the title, icons or structured data

Google keeps a cached copy of the title and favicon. To refresh it faster, open Google Search Console, inspect `https://kiankhayat.me/` and choose **Request indexing**.

## License

© Kian Khayat. All rights reserved.
