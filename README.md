# Montana 2026 — A Fly Fishing Travelogue

DePuy's Spring Creek and the Missouri River at Craig.
Luyen Chou & Thorne Sparkman — July 10–15, 2026.

## Structure

- `index.html` — the site (single file, hand-built)
- `img/` — trip photos
- `maps/` — illustrated SVG beat map (DePuy's), float line geometry (Missouri)
- `data/` — the source of truth
  - `itinerary.json` — reconstructed from Google Calendar
  - `conditions.json` — real USGS gauge data (flow + water temp) for the trip days
  - `moments.json` — the spine: every catch/photo as `{ts, lat, lon, river, species, fly, note}`

## Data provenance

Nothing in `data/` is invented. Each file carries `_source` and `_caveats` keys
noting where it came from and what's interpreted vs. stated. Confidence levels are
marked per-item. Verify interpreted spans against photo EXIF before publishing.

## Deploy

GitHub Pages from `main` / root. `noindex,nofollow` — shareable by link, not crawlable.
