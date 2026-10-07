# Norte Founder Network

Live view of the founders NDVC is sourcing for Norte Ventures (fall 2026): pipeline by stage, founder profiles, call notes and the team page.

## Files

- `index.html`: the whole site (no build step).
- `data.json`: every founder, the activity log and the "updated" date. **Edit this file to change what the site shows.**
- `art-*.png`: Norte illustrations.

## Updating the data

1. On the site, open the Team page and tap "Turn on editing".
2. Make your changes (notes, ratings, steps, calls, new founders).
3. When the site says it is read-only, tap "Copy data".
4. Paste it over `data.json` here and commit. Vercel redeploys in about a minute.

You can also edit `data.json` by hand. Each founder has a `stage` (`sourced`, `intro`, `reached`, `replied`, `talked`, `flagged`, `handed`), a `status` (`active` or `dropped`), a `rating` (0 to 5), `notes` and an optional `call`.
