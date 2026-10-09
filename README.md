# Limestone Plains Advisory: website

A static website (plain HTML and CSS, no build step). Host it free on Cloudflare Pages or Netlify by connecting this repository.

## Files
- `public/index.html`: the home page (all sections)
- `public/privacy.html`: privacy policy (draft, needs a lawyer's check)
- `public/assets/`: favicon, sample report PDF and its preview images
- `wrangler.jsonc`: tells Cloudflare Workers to serve the `public` folder

## Publish
1. Cloudflare Workers & Pages → this repository is connected as a Worker. Deploy command: `npx wrangler deploy` (reads `wrangler.jsonc`).
2. It goes live at `limestone-plains-website.<your-subdomain>.workers.dev`. Any change pushed to this repository republishes the site automatically.
3. Custom domain: in the Worker's Domains tab, add your domain (e.g. `limestoneplains.com.au`) and follow the DNS steps.

## Before you open for bookings (launch checklist)
Every claim on the site must be true on the day it goes live.

- [ ] Remove the orange **PREVIEW** ribbon (the `preview-ribbon` line at the top of `public/index.html`)
- [ ] Replace placeholders: email, phone, ABN (search for `[`)
- [ ] Certified Quantity Surveyor and Registered Planner reviewers engaged (the site says every report is reviewed)
- [ ] Professional indemnity insurance in place (the site says you hold it)
- [ ] Check with your employer that outside work is allowed
- [ ] Prices confirmed after interviews (Products section)
- [ ] Connect the enquiry form: create a free form endpoint (e.g. Formspree) and paste its URL into `data-endpoint=""` on the `<form id="enquiry">`
- [ ] Privacy policy reviewed by a lawyer; fill in the bracketed items
- [ ] Only mention the University of Canberra partnership once it is agreed in writing
- [ ] Set up a Google Business Profile pointing to the site
