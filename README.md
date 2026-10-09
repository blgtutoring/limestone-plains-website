# Limestone Plains Advisory: website

A static website (plain HTML and CSS, no build step). Host it free on Cloudflare Pages or Netlify by connecting this repository.

## Files
- `index.html`: the home page (all sections)
- `privacy.html`: privacy policy (draft, needs a lawyer's check)
- `assets/`: favicon, sample report PDF and its preview images

## Publish
1. Cloudflare Pages: Create a project → Connect to Git → pick this repository.
   Framework preset: **None**. Build command: *(leave empty)*. Output directory: `/`.
2. It goes live at `<project>.pages.dev`. Any change pushed to this repository republishes the site automatically.
3. Custom domain: in the Pages project, add your domain (e.g. `limestoneplains.com.au`) and follow the DNS steps.

## Before you open for bookings (launch checklist)
Every claim on the site must be true on the day it goes live.

- [ ] Remove the orange **PREVIEW** ribbon (the `preview-ribbon` line at the top of `index.html`)
- [ ] Replace placeholders: email, phone, ABN (search for `[`)
- [ ] Certified Quantity Surveyor and Registered Planner reviewers engaged (the site says every report is reviewed)
- [ ] Professional indemnity insurance in place (the site says you hold it)
- [ ] Check with your employer that outside work is allowed
- [ ] Prices confirmed after interviews (Products section)
- [ ] Connect the enquiry form: create a free form endpoint (e.g. Formspree) and paste its URL into `data-endpoint=""` on the `<form id="enquiry">`
- [ ] Privacy policy reviewed by a lawyer; fill in the bracketed items
- [ ] Only mention the University of Canberra partnership once it is agreed in writing
- [ ] Set up a Google Business Profile pointing to the site
