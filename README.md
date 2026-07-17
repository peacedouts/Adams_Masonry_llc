# Adams Masonry LLC — Business Website

**🔗 Live site: [adamsmasonryllc.com](https://adamsmasonryllc.com/)**

A single-page marketing website built for Adams Masonry LLC, a residential masonry business in Warsaw, Indiana. Hand-written static HTML, deployed on Cloudflare's static page hosting with a custom domain.

## What it does

The site gives a small local business a clean, fast web presence:

- **Services overview** — brick & block, chimneys & fireplaces, mailboxes, and columns
- **Photo gallery** of completed work
- **Customer testimonials** section
- **Contact section** with click-to-call links, a quote request form (with a honeypot field for basic spam protection), and service-area details
- **SEO basics** — descriptive title and meta description targeting local search

## Tech

| | |
|---|---|
| Frontend | Static HTML & CSS, single page, no frameworks or build step |
| Hosting | Cloudflare static page hosting |
| Domain & DNS | Custom domain on Cloudflare |
| Email | Cloudflare email address obfuscation on public contact links |

## Why static?

For a small business site, static hosting on Cloudflare means near-zero cost, no servers to patch or maintain, global CDN performance out of the box, and nothing to break. The whole site is one HTML file and a folder of images — easy to update, trivial to redeploy.

## Structure

```
.
├── index.html      # the entire site
├── photos/         # gallery images
└── *.jpg           # project photos (columns, fireplace, steps, mailboxes, entry)
```

## Deploying changes

Edit `index.html`, commit, and push — Cloudflare picks up the change and the site updates. No build pipeline required.
