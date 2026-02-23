# CLAUDE.md — Real O- Website

## Rules Source
- WAT framework rules: `WAT CLAUDE.md`
- Frontend design rules: `Web Design CLAUDE.md`

Both files are authoritative. Read them at the start of each session.

## Always Do First
- **Invoke the `frontend-design` skill** before writing any frontend code, every session, no exceptions.

## Stack
- Single `index.html`, all styles inline
- Tailwind CSS via CDN: `<script src="https://cdn.tailwindcss.com"></script>`
- Placeholder images: `https://placehold.co/WIDTHxHEIGHT`
- Mobile-first responsive

## Local Server
- Start: `node serve.mjs` (serves project root at `http://localhost:3000`)
- Always serve on localhost — never screenshot a `file:///` URL
- If server is already running, do not start a second instance

## Screenshot Workflow
1. `browser_resize` → `{ width: 1440, height: 900 }`
2. `browser_navigate` → `http://localhost:3000`
3. `browser_take_screenshot` → analyze directly
4. Fix mismatches, repeat from step 3
5. Final pass: resize to `{ width: 375, height: 812 }` for mobile

## Brand Assets
- Check `brand_assets/` before designing — use real assets over placeholders when available

## Project Structure
```
brand_assets/   # Logos, color palettes, fonts
tools/          # Python scripts for deterministic execution
workflows/      # Markdown SOPs
.tmp/           # Temporary/intermediate files (disposable)
.env            # API keys and secrets (never commit)
index.html      # Main site
serve.mjs       # Dev server
```

## Environment Variables
- All secrets in `.env` via `process.env`
- Never hardcode secrets
- Never overwrite `.env`
