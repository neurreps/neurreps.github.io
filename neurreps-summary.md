# NeurReps 2026 Site — Prototype Summary

**File:** `index.html` (+ `images/logo/` folder — keep alongside the HTML)

## What it is
Single-page static prototype for the NeurReps 2026 (NeurIPS, Sydney) homepage. Light theme, NeurReps blue (`#2B00FF`), Lato font, E8 Petrie projection as logo (nav, hero, splash screen). Sections: hero, mission, invited speakers, organizers, area chairs (TBD), CFP tracks, sponsors (TBD), past editions (empty, ready for entries).

## How to update content
Edit the data arrays near the bottom of the `<script>` tag — no other code changes needed:
- `SPEAKERS`, `ORGANIZERS` — add/edit `{ name, affiliation }` objects.
- `PAST_EDITIONS` — add `{ year, venue, proceedingsUrl }` objects as past years get archived; renders automatically once non-empty.

## Headshots
Drop an image into `images/people/` named as the person's slug: lowercase, spaces → hyphens (e.g. "Nina Miolane" → `nina-miolane.jpg`). Works with `.jpg`, `.jpeg`, `.png`, `.webp`. No matching file = automatic colored monogram fallback.

## Next steps (not yet done)
- Build remaining pages: Community, Speaker Series, Call for Papers, Resources, Proceedings, Past Editions (detail).
- Move content into `/data/*.yaml` files + set up a real repo (GitHub Pages under `github.com/neurreps`, custom domain `neurreps.org`).
- Fill in Area Chairs, Sponsors, Past Editions once finalized.
- Optionally get a smaller/vector source of the logo (current PNG is large).
