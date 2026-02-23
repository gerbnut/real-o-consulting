# Real O- Consulting

**Live site:** https://real-o-consulting.vercel.app

Operational consulting website for Real O-, a six-person firm founded by members of Northern Highlands Regional High School, Class of 2018.

## Stack

- Single `index.html` — no build step
- Tailwind CSS via CDN
- Google Fonts: Syne + DM Sans
- `serve.mjs` — local dev server (Node.js)

## Dev

```bash
node serve.mjs
# → http://localhost:3000
```

## Team

Jason Mindich · Henry Riccitelli · Matty "Mike" Ice · Ryan Starr · Evan Garbutt · Jack Mahan

## Deploy

Hosted on Vercel. Push to `main` and run:

```bash
vercel --prod --yes
```
