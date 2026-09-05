# Ocean-Side Dental — Dr. Irina Goncharuk

Static dental website for Dr. Irina Goncharuk, DDS, Brooklyn, NY.

## Scope
- English-first responsive site
- Ocean-Side Dental / Dr. Irina Goncharuk branding
- Services, doctor profile, reviews/trust section, contact and map
- Appointment UI with date/time selection
- Mobile sticky booking/call CTA
- Architecture ready for future multilingual expansion

## Important booking note
The site intentionally does **not** use the Agasi Dental booking endpoint. `BOOKING_API_URL` in `index.html` is blank until a dedicated booking backend / Google Apps Script for Ocean-Side Dental is created.

When the dedicated endpoint is ready, set:

```js
const BOOKING_API_URL = 'YOUR_OCEAN_SIDE_DENTAL_BOOKING_ENDPOINT';
```

Expected POST JSON:

```json
{
  "date": "YYYY-MM-DD",
  "time": "9:00 AM",
  "service": "Dental exam & cleaning",
  "name": "Patient Name",
  "phone": "+1...",
  "notes": "Optional"
}
```

The endpoint should return HTTP 2xx after saving the appointment. Do not connect this site to Agasi Dental's production data or calendar.

## Verified public practice information used in this first build
- Dr. Irina Goncharuk, DDS
- Ocean-Side Dental
- 3260 Coney Island Ave, Apt A4, Brooklyn, NY 11235
- (718) 891-0021
- 25+ years experience
- NYU, 2001
- Woodhull Medical Center residency
- Russian-speaking
- 4.7 Google rating / 50+ reviews
