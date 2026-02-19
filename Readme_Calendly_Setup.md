# Calendly setup for IT84 Support

Steps to set up Calendly for **samuel@it84.com.au**, connect Outlook, and link the booking page to this site. Calendly uses an **availability schedule** (you choose when you're available); Outlook busy times then block within those windows.

---

## 1. Create a Calendly account

1. Go to [calendly.com](https://calendly.com) and sign up (use **samuel@it84.com.au** or the shared IT84 email you prefer).
2. Complete profile: name, time zone (e.g. **Adelaide**), and any branding.

---

## 2. Set availability (when Samuel can be booked)

1. In Calendly, open **Availability** in the sidebar.
2. Under **Availability** (or **Default availability**):
   - Set **working hours** per day (e.g. Mon–Fri 9:00–17:00). Only these windows are offered to guests.
   - Use **+ Add hours** for split days (e.g. morning and afternoon blocks).
3. Set **Date range** (e.g. how far ahead guests can book).
4. **Buffer time** and **Maximum events per day** are optional.
5. Save.

This is the **availability calendar** approach: slots are only offered in the times you define here. You can change this schedule anytime to open or close booking windows.

---

## 3. Connect Outlook calendar

1. Go to **Availability** → **Calendar connections** (or **Integrations** → **Calendly for Outlook**).
2. Click **Connect** next to **Outlook Calendar** (or **+ Connect calendar**).
3. Sign in with **samuel@it84.com.au** when prompted and approve access.
4. Calendly will read the primary Outlook calendar and **block** any time marked Busy, Tentative, Away, or Working Elsewhere (you can change which statuses count under “What’s considered unavailable?”).
5. New Calendly bookings can be set to **add events to** this Outlook calendar so they appear in Samuel’s schedule.

**Notes:**

- Only the connected Outlook calendar’s busy/free is used; Calendly does not offer slots outside your **Availability** hours.
- So: **available to book = inside your Calendly availability AND free in Outlook.**

---

## 4. Create an event type

1. Go to **Event Types** → **+ Create**.
2. Name (e.g. *IT consultation* or *15-minute call*).
3. Set **Duration** (e.g. 15, 30, or 60 minutes).
4. Set **Location** (e.g. *Phone call*, *Microsoft Teams*, *In-person*).
5. Add **Description** and any **Invitee questions** if needed.
6. Under **Availability**, confirm it uses your default availability (or set a custom one).
7. Save.

---

## 5. Get the Calendly booking link

1. Open **Event Types** and click the event you want to use on the site.
2. Click **Share** (or the link icon). Copy the **Booking link** (e.g. `https://calendly.com/your-username/event-type`).
3. Use this URL in **booking.html** (see below).

---

## 6. Connect to this site (booking.html)

1. Open **booking.html** in this project.
2. Find the “Book an appointment” button and replace `href="#"` with the Calendly booking link, e.g.  
   `href="https://calendly.com/your-username/event-type"`.
3. Redeploy the site (e.g. to GoDaddy) so the updated link is live.

---

## Availability: how Calendly fits

- **Availability schedule**: You define when you’re available (days and hours). Only those windows are offered.
- **Outlook**: Within those windows, any time marked busy (or tentative/away, if you chose that) in the connected Outlook calendar is blocked.
- So Samuel can restrict bookings to specific times by adjusting his Calendly availability; he is not forced to have “all non‑busy time” bookable like in Microsoft Bookings.

---

## Checklist

- [ ] Calendly account created (samuel@it84.com.au or chosen email).
- [ ] **Availability** set (days and hours when Samuel accepts bookings).
- [ ] **Outlook calendar** connected; Calendly adds new events to Outlook.
- [ ] At least one **Event Type** created and shared.
- [ ] **booking.html** updated with the Calendly booking URL and redeployed.
