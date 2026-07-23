# Mobile 1 Audio — website

Static marketing site for **Mobile 1 Audio**, a car audio & customization shop at
867 S Dupont Hwy, New Castle, DE 19720 · (302) 268-6466.

Built the same way as the Allison's Automotive and Bleeks Automotive sites:
plain HTML/CSS/JS, no build step, deploys to GitHub Pages.

## Pages
- `index.html` — home (hero, services overview, why us, gallery preview, financing, reviews)
- `services.html` — full service list
- `about.html` — gallery + about
- `contact.html` — contact info, map, quote form
- `404.html`, `robots.txt`, `sitemap.xml`, `favicon.svg`

## Before it goes live — client to-do
1. **Photos** — drop real install photos in `/images/` and swap the placeholder
   tiles (`<span class="gallery-ph">…`) on `index.html` and `about.html` for
   `<img src="images/…" alt="…">`. Also add an `images/og-image.jpg` (1200×630)
   for social sharing.
2. **Confirm details** — verify the **unit number** at 867 S Dupont Hwy (listings
   show unit 2 vs 3), plus hours (currently Mon–Sat 9–6, Sun 12–5).
3. **Contact form** — replace `YOUR_FORM_ID` in `contact.html` with the client's
   [Formspree](https://formspree.io) endpoint. Until then the form politely tells
   visitors to call instead of failing.
4. **Domain** — replace every `REPLACE-WITH-DOMAIN.com` (canonical, OG tags,
   schema, sitemap, robots) with the real domain once purchased.
5. **Reviews** — swap the three placeholder testimonials on `index.html` for real
   quotes from the Google/Facebook page (do not invent customer names).
6. **Logo** — optional: add the shop's logo to the header in place of the
   equalizer mark if they have one.

## Deploy (GitHub Pages, same as the other client sites)
```
git init
git add .
git commit -m "Initial Mobile 1 Audio site"
# create repo under jovensanghera307-ux, push, enable Pages on the default branch
```

## Preview locally
Any static server works, e.g.:
```
npx serve .
```
