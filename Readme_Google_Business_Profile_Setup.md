# Google Business Profile setup for IT84 Support

Steps to create and verify a **Google Business Profile** (formerly Google My Business) so IT84 Support appears in Google Search and Maps. Once set up, you can add the profile link to the website (see TODO: confirm if Google Business Profile link should be added).

---

## 1. Sign in and go to Business Profile

1. Go to [business.google.com](https://business.google.com).
2. Sign in with the **Google account** you want to manage the business (e.g. **samuel@it84.com.au** if using Google Workspace, or a dedicated IT84 Google account).
3. If prompted, accept the **Google Business Profile** terms.

---

## 2. Add or claim the business

1. Click **Add your business to Google** (or **Manage now** if the business already exists).
2. Enter the **business name** (e.g. **IT84 Support**).
3. Choose the correct **business category** (e.g. *IT services and IT consulting*, or *Computer support and services*). This affects how you appear in search.
4. Choose whether you have a **location customers visit** (e.g. office) or **serve customers at their location** (service area), or both.
   - For a **service area** business: add regions (e.g. Hahndorf, Angle Vale, McLaren Vale, Murray Bridge, Nuriootpa) so you show up for “IT support near [suburb]”.
5. Enter the **business address** (if you have a physical location). For service-area only, you can hide the address from the public and show only service areas.
6. Add **phone number** and **website** (e.g. your live site URL such as `https://it84support.com.au` or current Netlify URL).
7. Complete any extra prompts (e.g. business hours, attributes).

---

## 3. Verify the business

Google requires **verification** before the profile goes fully live.

1. Choose **verification method**. Common options:
   - **Postcard**: Google sends a code to your business address. Enter the code in the Business Profile dashboard when it arrives (often 5–14 days).
   - **Phone**: Sometimes offered for eligible businesses; you receive a code by call or SMS.
   - **Email**: For some businesses; code sent to a business email.
2. Request the verification (e.g. request postcard) and wait for the code.
3. In [business.google.com](https://business.google.com), open the verification step and enter the **verification code**.
4. After approval, the profile can appear in Search and Maps.

**Tip:** Use the exact business address and ensure mail can be received there (postcard must be deliverable).

---

## 4. Complete the profile

After verification:

1. **Business info**
   - **Description**: Short summary of IT84 Support (support, Microsoft 365, consulting, regions served).
   - **Hours**: Opening hours if you have a physical location; otherwise set “By appointment” or service hours if relevant.
   - **Attributes**: Add any that apply (e.g. “On-site services”, “Remote support”).
2. **Photos**
   - Add **logo** and **cover** image; add photos of team, office, or equipment if desired (improves trust and visibility).
3. **Services**
   - List main services (e.g. Microsoft 365 support, on-site support, consulting) so they show on the profile.
4. **Products** (optional)
   - Add key offerings if you use this section.
5. **Posts** (optional)
   - Use posts for updates, offers, or events to keep the profile active.

---

## 5. Link the profile to the website

1. In the Business Profile dashboard, copy the **profile link** (e.g. “Share profile” or the URL shown when you click “View on Search”).
2. In this project, add the link where appropriate (e.g. footer or contact section in **index.html**, or a dedicated “Find us on Google” button). Coordinate with the TODO item: *Confirm if Google Business Profile link should be added*.
3. Redeploy the site after updating the link.

---

## 6. Delegate Manager (editor) role to graham@grahamcrispin.com

To let **graham@grahamcrispin.com** edit the Business Profile (info, posts, replies) without owner-level control:

1. Go to [business.google.com](https://business.google.com) and open the IT84 Support **Business Profile**.
2. In the dashboard, open the **Users** (or **People**) section (menu or **Settings** → **Users**).
3. Click **Add users** (or **Invite users**).
4. Enter **graham@grahamcrispin.com**.
5. Set the role to **Manager**.
   - **Manager** can: edit business info, post updates, reply to reviews and Q&A, view insights. Cannot: remove the owner, transfer ownership, or delete the profile.
6. Send the invite. Graham will receive an email and must accept to get access.

**Note:** Graham must use a Google account with that email (or add it to their Google account). After accepting, they can manage the profile from [business.google.com](https://business.google.com) or the Google Business Profile app.

---

## 7. Ongoing management

- **Google Business Profile app** (iOS/Android): Use it to reply to reviews, update hours, and add quick updates.
- **Reviews**: Respond to reviews to build trust and show engagement.
- **Insights**: In the dashboard, check how customers find you (Search vs Maps) and what actions they take (website visits, calls, direction requests).

---

## Checklist

- [ ] Google account chosen for managing the business (e.g. samuel@it84.com.au or IT84 Google account).
- [ ] Business added at [business.google.com](https://business.google.com) with correct name, category, and location/service area.
- [ ] Phone number and website URL added.
- [ ] Verification requested and completed (postcard/phone/email).
- [ ] Description, hours, attributes, and services filled in.
- [ ] Logo and at least one cover/photo added.
- [ ] Profile link added to the website (after confirmation) and site redeployed.
- [ ] **Manager** role delegated to **graham@grahamcrispin.com** (Users → Add users → Manager).
