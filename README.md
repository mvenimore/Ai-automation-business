# Autonova — AI Automation Landing Page

A clean, modern landing page for the Autonova AI automation business, with a built-in waitlist signup form.

## Setup

### 1. Host the page

Deploy `index.html` anywhere static hosting works:

- **Netlify**: drag-and-drop the file at [netlify.com/drop](https://netlify.com/drop)
- **Vercel**: `npx vercel --yes` from this directory
- **GitHub Pages**: push to a repo and enable Pages in Settings

### 2. Connect the waitlist (Formspree)

The form submits to [Formspree](https://formspree.io) — a free form backend that emails you every signup.

1. Sign up at [formspree.io](https://formspree.io) (free tier: 50 submissions/month)
2. Create a new form and copy the form ID (looks like `xrgjabc`)
3. Open `index.html` and replace `YOUR_FORM_ID` on this line:
   ```js
   const FORMSPREE_ID = 'YOUR_FORM_ID';
   ```
4. Redeploy — signups will now land in your inbox

> **Upgrade tip**: For unlimited signups, upgrade Formspree or switch to [EmailOctopus](https://emailoctopus.com) (free up to 2,500 subscribers) with a webhook.

## Customizing

- **Colors**: Edit the CSS variables in `:root` at the top of `index.html`
- **Copy**: All text is inline HTML — search for what you want to change
- **Waitlist count**: Update "500+" in the hero's social proof line
- **Company name**: Replace "Autonova" with your preferred name throughout
