# Okandaba website

A one-page, mobile-first static site for Okandaba Holdings, built from the approved design. No build step, no database: plain HTML, CSS and a small JavaScript file.

## Files

- `index.html`: the whole page (content, SEO tags, Google business details).
- `assets/css/styles.css`: styles, written phone-first (base rules for phones, then 640px / 900px / 1180px breakpoints).
- `assets/js/main.js`: mobile menu, price tabs, footer year. The page still works without it.
- `assets/img/`: optimised photos and logos (WebP for logos, JPG for photos).
- `favicon.png`, `assets/img/apple-touch-icon.png`, `assets/img/og-image.jpg` (link preview on WhatsApp/Facebook).

## Updating content

- **Prices:** in `index.html`, search for `panel-couches`, `panel-mattresses` and so on. Each line is `<div><dt>Item</dt><dd>Price</dd></div>`.
- **Phone numbers:** WhatsApp links use `https://wa.me/27780514145`; the call button uses `tel:+27691110191`.
- **Photos:** replace a file in `assets/img/` with one of the same name (square photos work best for services).

## Publishing

Any static host works. Free options:

1. **Netlify Drop:** go to app.netlify.com/drop and drag this folder in. You get a live link in seconds; connect a domain later.
2. **Cloudflare Pages** or **Vercel:** create a project and upload the folder (or connect a GitHub repo).
3. **Existing cPanel hosting:** upload the folder contents to `public_html`.

Before launch, set the full domain in the `og:image` tag (for example `https://okandaba.co.za/assets/img/og-image.jpg`) so link previews show the image.
