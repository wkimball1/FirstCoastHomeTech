# First Coast Home Tech — Website

Professional, mobile-first website for First Coast Home Tech: friendly in-home technology support serving Nassau County and the First Coast, Florida.

## Quick start

1. **Preview locally:** Open `index.html` in a browser, or use a simple local server:
   ```bash
   npx serve .
   ```
2. **Deploy:** Upload the entire folder to any static host (Netlify, Vercel, GitHub Pages, or your hosting provider). No build step required.

## Before going live

- **Phone number:** The site uses (904) 335-8766. To change it, search for `335-8766` and `19043358766` in the HTML files.
- **Contact form (you get emails, your email is never shown):** The form sends submissions via Formspree. See **[CONTACT_FORM_SETUP.md](CONTACT_FORM_SETUP.md)** for step-by-step setup. You add your email only in the Formspree dashboard — it never appears on the site.
- **Your domain:** Replace `https://www.firstcoasthometech.com` with your real site URL in: all four HTML files (canonical + og:url), `sitemap.xml`, and `robots.txt`. Search for `firstcoasthometech.com` to find every instance.
- **Google Map:** In [Google Maps](https://maps.google.com), search for your business or “Nassau County, FL,” click **Share** → **Embed a map**, and replace the iframe in `contact.html` with the code Google provides.

## Structure

- `index.html` — Home
- `services.html` — Services and pricing
- `about.html` — About / founder story
- `contact.html` — Contact form, call/text, map
- `css/styles.css` — All styles (mobile-first)
- `js/main.js` — Mobile menu and sticky call button

## SEO

- **On every page:** Unique title, meta description, one H1, canonical URL, Open Graph and Twitter Card meta (for when links are shared).
- **Homepage:** JSON-LD LocalBusiness schema (name, phone, service areas) so search engines can show your business in local results.
- **sitemap.xml** and **robots.txt** are included; update the domain in both when you go live.
- **Keywords** are used naturally in copy: in-home tech support First Coast, Amelia Island tech help, Fernandina Beach computer help, Nassau County Wi-Fi troubleshooting, smart home setup First Coast, local tech support near me.

---

**First Coast Home Tech** — *Friendly, in-home tech help for real life.*
