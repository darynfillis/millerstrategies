# YouTube Embed Production Fix

## What changed

- Jeff Miller's profile now uses the standard YouTube iframe embed rather than the IFrame Player API.
- The iframe includes `referrerpolicy="strict-origin-when-cross-origin"`.
- Every HTML page includes:
  `<meta name="referrer" content="strict-origin-when-cross-origin">`
- Added deployment header config files:
  - `_headers` for Netlify / Cloudflare Pages style static hosting
  - `vercel.json` for Vercel
  - `.htaccess` for Apache hosting

## Video

Embed URL:
https://www.youtube.com/embed/srJpjKBlCJY?si=8UQs35iS0fynkJLc

Fallback URL:
https://www.youtube.com/watch?v=srJpjKBlCJY

## Production checklist

If the video still fails in production, check the live response headers and make sure the host is not sending:

`Referrer-Policy: no-referrer`

If there is a Content-Security-Policy header, it must allow YouTube frames:

`frame-src https://www.youtube.com https://www.youtube-nocookie.com;`

or equivalent.
