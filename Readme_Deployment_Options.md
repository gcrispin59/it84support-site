# Readme_Deployment_Options

This document outlines options for hosting and deployment, with steps for each path.

---

## Plan A — Move hosting to GoDaddy (static hosting)

Goal: host the static site directly on GoDaddy.

**Steps**
1. Export the latest site build (current repo contents are already static).
2. In GoDaddy:
   - Open hosting control panel.
   - Upload all site files to the web root (usually `public_html`).
3. Confirm GoDaddy uses `index.html` as the default.
4. Verify pages load:
   - `index.html`, `booking.html`, `testimonials.html`, service pages
5. Update `robots.txt` and `sitemap.xml` if the domain changes.
6. Optional: enable HTTPS in GoDaddy.

**Pros**
- Simple and stays in GoDaddy.
- No extra services.

**Cons**
- No CI/CD from GitHub.
- Manual upload each change.

---

## Plan B — Host on Google Sites

Goal: use Google Sites as the hosting platform.

**Steps**
1. Recreate pages in Google Sites (manual migration).
2. Add pages for Services, Testimonials, Booking, etc.
3. Add embeds (RSS ticker may need to be simplified).
4. Map custom domain in Google Sites.
5. Update DNS in GoDaddy to point to Google Sites.

**Pros**
- Easy editing in browser.
- Good for non-technical owners.

**Cons**
- Rebuild required (not a direct deploy).
- Limited control over HTML/CSS.
- RSS ticker and advanced features may not work.

---

## Plan C — Keep Netlify + point GoDaddy DNS to Netlify

Goal: stay on Netlify (best for GitHub deploys) while using GoDaddy domain.

**Steps**
1. Create/transfer Netlify site to an IT84Support-owned Netlify account.
2. Connect GitHub repo to Netlify (auto-deploy on push).
3. Add custom domain in Netlify (e.g., `it84support.com.au`).
4. In GoDaddy DNS:
   - Add `A` record(s) pointing to Netlify IPs
   - Add `CNAME` for `www` -> Netlify site
5. Verify SSL certificate in Netlify.
6. Test all pages and links.

**Pros**
- Automatic deploys from GitHub.
- Best performance and flexibility.
- Easy rollback and preview deploys.

**Cons**
- Requires Netlify account and DNS changes.

---

## Moving to an IT84Support-owned Netlify account (Plan C detail)

**Steps**
1. Create a new Netlify account for IT84Support.
2. Invite the current owner or transfer site ownership.
3. Connect the GitHub repo:
   - Choose `gcrispin59/it84support-site`
   - Build command: none
   - Publish directory: repo root
4. Enable auto-deploys on push.
5. Add the custom domain.

**Keeping GitHub links intact**
- No changes needed; the repo remains the same.
- Netlify just re-connects to the existing repo.
