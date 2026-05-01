# OG Card Production Fix

## What changed

The OG image is now referenced from the root of the domain:

`https://millerstrategies.com/og-card.jpg`

This is intentionally simpler than a nested asset path because social crawlers are more reliable when the image has a short, direct, public URL.

## Files added

- `/og-card.jpg`
- `/og-card.png`
- `/assets/og/miller-strategies-og-card.jpg`
- `/assets/og/miller-strategies-og-card.png`

## Required upload

Upload these files to production:

- `og-card.jpg`
- `og-card.png`
- the updated HTML files
- optionally the `/assets/og/` folder as a backup

## Test after upload

Use:
- LinkedIn Post Inspector
- Facebook Sharing Debugger
- X Card Validator

If the old image still appears, scrape/debug the URL again. Social platforms cache OG cards aggressively.
