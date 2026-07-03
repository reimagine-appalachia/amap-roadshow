# Summer 2026 Manufacturing Roadshow — Resource Site

A simple static website (no accounts, no personal data collection except an optional
email signup) for ReImagine Appalachia's Summer 2026 Manufacturing Roadshow Series.

## Files

- `index.html` — home page: stop overview, about blurb, email signup
- `agenda.html` — full agenda for all 5 stops
- `speakers.html` — all 22 speakers with organization and which stop(s) they're at
- `resources.html` — partner org descriptions and resource links
- `about.html` — A-MAP vision, 10 pillars, why attend, what's next
- `styles.css` — shared styling (ReImagine Appalachia teal/gold brand)
- `assets/hero-bg.jpg` — background photo used on the home page hero
- `assets/A-MAP-One-Pager.pdf` — the original one-pager, offered as a download
- `assets/ra-logo.png` — real ReImagine Appalachia logo (from the file you attached)
- `assets/amcc-logo.png` — real AMCC logo (from the file you attached)
- `assets/logo.png`, `assets/img_0.jpeg`, `assets/img_1.png`, `assets/logo_preview_TEMP.png`,
  `assets/amcc_preview_TEMP.png` — earlier extracted/recreated logo attempts, no longer
  used anywhere on the site, safe to ignore or delete

## Deploying to Cloudflare Pages (free)

1. Go to the [Cloudflare dashboard](https://dash.cloudflare.com/) → **Workers & Pages** → **Create** → **Pages** → **Upload assets**.
2. Drag this whole folder in (or zip it and upload the zip).
3. Give it a project name — Cloudflare will assign a free `*.pages.dev` URL immediately.
4. Optional: add a custom domain under the project's **Custom domains** tab if you have one.
5. To make future edits live, just re-upload the folder (or connect a GitHub repo for automatic deploys if you'd rather work that way).

No build step, no server, no database — it's just static files.

## Before you publish — a few things to fill in

**1. Email signup form — done.** The "Stay updated" form on the home page now posts to
your real Formspree endpoint (`https://formspree.io/f/mbdvppaw`, "A-MAP and Roadshow
Updates" form). Test it once live to confirm submissions land where you expect.

**2. Links still marked "Coming Soon."** A few resources were referenced in the source
materials as clickable text but without a URL. What's still outstanding on
`resources.html`: AMCC slides, the AMCC Monday Call/weekly newsletter signup, and the
True Pigments website. Search for `class="link-btn pending"` in `resources.html` to
find and replace each one.

**3. Phone number.** The source one-pager had a placeholder phone number
(123-456-7890) that was clearly not real, so I left it off the site. Add a real one to
the footer in each HTML file if you have one.

**4. Virtual stop & summit details.** The September 8 virtual stop and the closing
summit don't have full agendas or registration links yet — `agenda.html` currently
shows "Registration Coming Soon" for both. Update those once details are set.

## Why this version is low-risk

No accounts, no login, no AI processing of personal data, no participant bios or
profiles. The only data collected is an optional email address for update
notifications, clearly disclosed and opt-in.
