# First Coast Home Tech — Website

Professional, mobile-first website for First Coast Home Tech: friendly in-home technology support serving Nassau County and the First Coast, Florida.

## Deployment

The site is automatically deployed to GitHub Pages via the included workflow (`.github/workflows/static.yml`) whenever changes are pushed to the `main` branch.

### Custom domain (firstcoasthometech.com)

A `CNAME` file is included in this repository so GitHub Pages serves the site at **firstcoasthometech.com**. You also need to configure DNS at your domain registrar:

1. **Apex domain (`firstcoasthometech.com`)** — Add four `A` records pointing to GitHub's IPs:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
2. **`www` subdomain** — Add a `CNAME` record:
   ```
   www  →  wkimball1.github.io
   ```
3. **Enable HTTPS** — In your GitHub repository go to **Settings → Pages** and tick *Enforce HTTPS* once DNS has propagated.

> DNS changes can take up to 24–48 hours to propagate worldwide.

---

## Quick start

1. **Preview locally:** Open `index.html` in a browser, or use a simple local server:
   ```bash
   npx serve .
   ```
2. **Deploy:** Upload the entire folder to any static host (Netlify, Vercel, GitHub Pages, or your hosting provider). No build step required.

## Before going live

- **Phone number:** Replace `(904) 555-0123` and `+19045550123` with your real number in all HTML files (search for `904` and `19045550123`).
- **Contact form:** Sign up at [Formspree](https://formspree.io), create a form, and replace `YOUR_FORM_ID` in `contact.html` with your form ID. Or connect another form service (Netlify Forms, etc.).
- **Google Map:** In [Google Maps](https://maps.google.com), search for your business or “Nassau County, FL,” click **Share** → **Embed a map**, and replace the iframe in `contact.html` with the code Google provides.

## Structure

- `index.html` — Home
- `services.html` — Services and pricing
- `about.html` — About / founder story
- `contact.html` — Contact form, call/text, map
- `css/styles.css` — All styles (mobile-first)
- `js/main.js` — Mobile menu and sticky call button

## SEO

Pages include title tags, meta descriptions, and H1s. Target terms are used in copy: in-home tech support First Coast, Amelia Island tech help, Fernandina Beach computer help, Nassau County Wi-Fi troubleshooting, smart home setup First Coast, local tech support near me.

---

**First Coast Home Tech** — *Friendly, in-home tech help for real life.*
