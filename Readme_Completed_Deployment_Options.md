# Readme_Deployment_Options

## Not Chosen Plan A — Move hosting to GoDaddy (static hosting)

## Not Chosen Plan B — Host on Google Sites

## Plan C — Keep Netlify + point GoDaddy DNS to Netlify

Goal: stay on Netlify (best for GitHub deploys) while using GoDaddy domain.

**Steps**
1. Create/transfer Netlify site to an IT84Support-owned Netlify account.
2. Connect GitHub repo to Netlify (auto-deploy on push).
3. Add custom domain in Netlify (e.g., `it84support.com.au`).
4. 
5. In GoDaddy DNS:
   - Add `A` record(s) pointing to Netlify IPs
   - Add `CNAME` for `www` -> Netlify site
6. Verify SSL certificate in Netlify.
7. Test all pages and links.

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
