# Rai Scaling website

Static site for [raiscaling.com](https://raiscaling.com) — two self-contained HTML pages, no build step.

- `index.html` — homepage
- `results.html` — served at `/results` (see `vercel.json` → `cleanUrls`)

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

## Deploying

This repo is meant to be connected to [Vercel](https://vercel.com) with zero build configuration (it's plain
HTML/CSS/JS, no framework). Once the GitHub repo is connected to a Vercel project, every push to `main`
auto-deploys.

## Editing

Both pages are single self-contained files (styles and scripts inline). Find the "Book a Free Call" links by
searching for `book-a-call` — there's an HTML comment above the final CTA section in each file marking where to
swap in the real GoHighLevel calendar URL once it's ready.
