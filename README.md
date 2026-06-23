# REI Hospitality — Website

Static single-page marketing site for **reihospitality.com**. Plain HTML/CSS, no build step. Hosted on GitHub Pages.

## Files
- `index.html` — the whole site (inline styles, one small script for the contact form).
- `CNAME` — custom domain for GitHub Pages (`reihospitality.com`).
- `robots.txt`, `sitemap.xml` — basic SEO.

## Contact form (Formspree)
The form posts to Formspree via AJAX (`https://formspree.io/f/xnjkqedr`) and shows the on-page
"Got it. Talk soon." confirmation on success. Submissions currently route to
`ellis@ctbackofficesolutions.com`; switch the destination in the Formspree form settings once
`ellis@reihospitality.com` is set up as a verified linked email.

## Deploy
GitHub Pages serves `index.html` from the default branch. Custom domain is set by the `CNAME` file plus DNS records at GoDaddy:
- `A` records for `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- `CNAME` for `www` → `<github-username>.github.io`
