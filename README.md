# Norte Founder Network

A small static site the Notre Dame Venture Capital (NDVC) team uses to track early-stage founders it sources for Norte Ventures (fall 2026). It shows the pipeline by stage, founder profiles, call notes and a team page.

**Why:** seven student members each sourced founders for Norte. A shared page kept the pipeline, ratings and next steps in one place instead of scattered across chats and sheets.

**Status:** in use during the fall 2026 sourcing round. Last data update: Oct 7, 2026 (31 founders in the pipeline, outreach starting).

## Files

- `index.html`: the whole site (plain HTML/JS, no build step).
- `data.json`: every founder, the activity log and the "updated" date. **Edit this file to change what the site shows.**
- `art-*.png`: Norte illustrations.

## Run locally

Open `index.html` through any static server (the page loads `data.json`):

```bash
npx serve .
```

## Updating the data

1. On the site, open the Team page and tap "Turn on editing".
2. Make your changes (notes, ratings, steps, calls, new founders).
3. When the site says it is read-only, tap "Copy data".
4. Paste it over `data.json` here and commit. Vercel redeploys in about a minute.

You can also edit `data.json` by hand. Each founder has a `stage` (`sourced`, `intro`, `reached`, `replied`, `talked`, `flagged`, `handed`), a `status` (`active` or `dropped`), a `rating` (0 to 5), `notes` and an optional `call`.
