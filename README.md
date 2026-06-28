# Koha Events Manager Plugin

A Koha plugin that lets librarians manage library events from the
staff interface and display them on the OPAC as a styled, customizable
widget — colors, fonts, images, borders, layout, and placement are all
configurable from the staff client, no template editing required.

Compatible with Koha **20.05 and newer**, including Koha 23.05+ / 25.07's
"HTML customizations" screen.

## Features

- Full event CRUD (create/edit/delete) from **Tools → Events Manager**
- Upload an image per event (stored in the database — no file server
  config needed) or link to an external image URL
- Per-event accent color and font, with site-wide defaults
- Configurable widget heading (e.g. "Upcoming Events", "What's On")
- Three layouts: simple list, vertical scroll, or horizontal carousel —
  with adjustable width/height and auto-scroll speed
- Border style, corner roundness, and shadow controls
- Two placement methods: automatic (under the OPAC search box, zero
  setup) or a copy-paste embed snippet for exact placement via Koha's
  HTML customizations / OPAC system preferences
- A live, in-staff-client preview plus a per-event "OPAC status"
  diagnostic (Showing / Draft / Ended, with the reason)
- Responsive layout and accessibility-minded markup (ARIA regions,
  proper headings, descriptive alt text, visible focus outlines)
- Self-healing database schema — safe to upgrade in place
- CSRF-protected forms, friendly error pages instead of raw HTTP 500s

## Quick start

1. Download `Koha-Event-Manager-Plugin.kpz` from
   [Releases](../../releases) (...Latest...).
2. Enable the `KohaPlugins`.
3. **Administration → Manage plugins → Upload plugin** → upload the `.kpz`.
4. Open **Tools → Events Manager**, add an event, and check the Live
   preview.
5. Turn on **Automatically show on the OPAC home page** in Widget
   settings, save, and refresh your OPAC.



