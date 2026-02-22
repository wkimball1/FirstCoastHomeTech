# Contact form setup (emails to you — your email never appears on the site)

The contact form uses **Formspree**. Formspree sends each submission to **your email**. Your email is only entered in the Formspree dashboard, so it is **never shown on the website** or in the HTML.

## Steps

1. **Sign up:** Go to [formspree.io](https://formspree.io) and create a free account.

2. **Create a form:** Click “New Form.” Give it a name (e.g. “First Coast Home Tech contact”).

3. **Set your email:** In the form settings, set the notification email to the address where you want to receive messages (e.g. your Gmail). This is only stored in Formspree — visitors never see it.

4. **Get your form ID:** Formspree will show a form endpoint like:
   `https://formspree.io/f/xyzabcde`
   The form ID is the part after `/f/` (e.g. `xyzabcde`).

5. **Update the website:** Open `contact.html` and find:
   ```html
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
   Replace `YOUR_FORM_ID` with your actual form ID (e.g. `xyzabcde`), so it looks like:
   ```html
   action="https://formspree.io/f/xyzabcde"
   ```
   Save the file.

6. **Test:** After you deploy the site, submit the contact form. You should get an email at the address you set in Formspree.

## Optional Formspree settings

- **Auto-respond:** In Formspree you can turn on “Auto-respond” and set a message so the customer gets a “Thanks, we’ll be in touch” email.
- **Spam filtering:** Formspree’s free plan includes basic spam filtering.

Your email stays private: it’s only in your Formspree account, not on the site.
