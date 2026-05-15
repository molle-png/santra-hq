# santra HQ — Weekly Memo Assistant

Chat-driven intake for the santra weekly memo. Five sections, two minutes, one copyable block ready to paste into Telegram.

Live page: [https://molle-png.github.io/santra-hq/](https://molle-png.github.io/santra-hq/)

## What it asks

1. **Output this week** — what shipped
2. **In flight** — what's active, with dates
3. **Blockers** — what's stuck, who needs to act
4. **Q2 alignment** — 1–5 self-rating against three OKRs (Seed Round, +100k MRR, Moments by Santra)
5. **Next 7 days** — top three commitments

The final memo is rendered as a monospace block with a one-tap copy button. Output is plain text — paste straight into Telegram, email, or Notion.

## Why it's a single static HTML file

No build step, no server, no analytics, no data leaves the browser. State lives in memory for the duration of the session and is discarded on refresh. The page works offline once loaded (the only external request is Google Fonts on first paint).

## Hosting

Served from GitHub Pages off the `main` branch root.

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```
