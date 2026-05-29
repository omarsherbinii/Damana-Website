# Damana Website — Deployment Guide

## Files
- `index.html` — Main landing page (hero, demo, how it works, pre-registration)
- `demo.html` — Standalone transaction link demo (all 5 party views)

---

## Deploy in 30 minutes (Free)

### Step 1 — GitHub (5 min)
1. Go to https://github.com and create a free account
2. Click **New repository** → name it `damana-website` → Public → Create
3. Click **uploading an existing file**
4. Drag and drop both `index.html` and `demo.html`
5. Click **Commit changes**

### Step 2 — Vercel (5 min)
1. Go to https://vercel.com → Sign up with GitHub
2. Click **Add New Project** → Import `damana-website`
3. Leave all settings default → click **Deploy**
4. Your site is live at `damana-website.vercel.app` in ~60 seconds

### Step 3 — Custom domain (10 min)
1. Buy `damana.link` at https://namecheap.com (~$15/year)
2. In Vercel: go to your project → **Settings** → **Domains**
3. Add `damana.link` → Vercel gives you DNS records
4. In Namecheap: go to **Advanced DNS** → add the records Vercel gives you
5. Wait 10-30 minutes → your site is live at damana.link

### Step 4 — Real form submissions
Replace the fake form with Tally (free):
1. Go to https://tally.so → Create account
2. Build a form with the same fields (business name, email, phone, category, monthly orders, pain point)
3. Copy the embed code → replace the `<div class="reg-form">` section in index.html
4. All submissions go to your Tally dashboard automatically

### Step 5 — Professional email
1. Go to https://zoho.com/mail → Free plan
2. Add your domain `damana.link`
3. Follow DNS setup → you get `hello@damana.link`

### Step 6 — Analytics
Add before `</head>` in both files:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_ID');
</script>
```
Get your ID at https://analytics.google.com

---

## What to update before going live

In `index.html`:
- Replace `hello@damana.link` in footer with your real email
- Connect Tally form for real registrations

In `demo.html`:
- The demo is ready as-is — share `damana.link/demo.html` in validation calls

---

## Sharing in validation calls
Send merchants this link: `damana.link/demo.html`
- Tell them to click each party tab (Buyer, Merchant, PSP, Courier, Bank)
- The 48h timer counts down in real time
- The return flow is fully interactive
- All 5 party views show exactly what they'd see in production

---

## Next steps after launch
1. Post the link in merchant WhatsApp groups and Facebook e-commerce communities
2. Share `damana.link` on LinkedIn with the headline: "We're building trust infrastructure for Egyptian e-commerce — join the waitlist"
3. Send the demo link to every merchant you've already spoken to
4. Track registrations in Tally → follow up within 48h as promised
