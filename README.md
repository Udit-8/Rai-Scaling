# Rai Scaling website

Static site for [raiscaling.com](https://raiscaling.com) — one self-contained HTML page, no build step.

- `index.html` — homepage
- `privacy.html` — privacy policy, served at `/privacy` (linked from the footer and used for Meta lead forms)
- `images/` — ad examples and client dashboard screenshots used on the homepage
- `/results` redirects to the homepage's previous-work section (see `vercel.json`)

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

The page is a single self-contained file (styles and scripts inline), with images in `images/`. Find the "Book a Free Call" links by
searching for `book-a-call` — there's an HTML comment above the final CTA section in each file marking where to
swap in the real GoHighLevel calendar URL once it's ready.
