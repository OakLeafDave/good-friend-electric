# Good Friend Electric — Website

A fast, single-file static site for **Good Friend Electric** — a family-owned
electrical & lighting distributor serving the Jersey Shore since 1937 (six
branches across Ocean & Monmouth County, NJ). Built by Oak Leaf Media as a
modern replica/pitch of goodfriendelectric.com.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire site (HTML + CSS + JS inline; only external dep is Google Fonts) |
| `assets/logo.gif`, `logo@2x.gif` | The real 89th-anniversary logo (pulled from their live site) |
| `assets/store-hours.jpg` | Their store-hours graphic (reference; hours are rebuilt in HTML) |
| `favicon.svg` | Site icon (lightbulb-in-diamond mark) |
| `site.webmanifest` | PWA / add-to-homescreen metadata |
| `robots.txt`, `sitemap.xml` | SEO crawler files |
| `netlify.toml` | Deploy + security headers config |

## Local preview

Registered in `~/.claude/launch.json` as **good-friend-electric** on **port 8439**
(`python3 -m http.server 8439 --directory ~/good-friend-electric`).

## Company facts (as replicated)

- Founded **1937** by Manny & Lillian Goodfriend, Main St, Toms River. Rosen family since 1949; incorporated as Good Friend Electric 1957. Four generations — today led by President David Rosen & son Ethan Rosen.
- **6 branches:** Toms River (HQ, 265 Route 37 E, 732-349-4100), Lacey (403 Route 9, 609-693-8100, est. 1987), Brick (534 Brick Blvd, 732-920-7100, est. 1989), Manahawkin (325 Route 72 E, 609-978-9100, est. 1995), Lakewood (121 E County Line Rd, 732-942-3100, est. 1998), Wall (1245 18th Ave, 732-456-5100, est. 2020).
- **Hours:** Mon–Fri 7:30a–5p all locations. Sat: Toms River 8a–5p; all others 8a–12p.
- Brand: royal blue `#1c3f94` + gold `#f6c945`. NAED member. 350+ yrs combined team experience.

## Before going live — checklist

1. **Wire up the contact form.** In `index.html`, find `const FORM_ENDPOINT = ''`
   near the bottom `<script>`. Create a free form at [formspree.io](https://formspree.io)
   and paste the endpoint URL there.
2. **Add `og-image.jpg`** (1200×630 social-share image) — referenced by the Open Graph tags.
3. **Verify zip codes** — the per-branch ZIPs were inferred from town; confirm before publishing.
4. **Confirm Saturday hours / product mix** with the client — pulled from their current site 2026-07-06.
