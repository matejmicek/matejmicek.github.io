# Trail Atlas

Source-linked planning for Czechia, the Alps and nearby countries: events starting **22 September 2026 through 31 December 2027**, plus clearly separated undated 2027 watchlists.

Snapshot researched **22 September 2026**. 153 event editions (119 event families), 10 countries: 69 organiser-confirmed dates, 7 provisional calendar dates, 77 date-TBA entries. 110 editions are in Czechia. Broad coverage, not an exhaustive registry of every local race. No automatic refresh.

## Use

- Race index, year calendar with month detail, and a drive-time versus longest-course chart.
- Search, country, distance, drive-time, format, year, confirmed-date and shortlist filters.
- Per-edition source links, organiser/registration links, published GPX or route pages, team rules and course provenance.
- Shortlist saved only in browser local storage. JSON download and ICS export; undated entries excluded, calendar-only dates exported as tentative.

## Data conventions

`races.json` is the public research dataset. Every record contains sources and a verification date. `startDate`/`endDate` are ISO dates; null means unknown. Multi-distance festivals are one edition, with their event/race window; check the chosen distance's start time. A watchlist month is a prior-edition planning guide, not a future date.

`courseReference` marks prior-edition course details independently of date confirmation. Direct GPX downloads, archives, viewer pages and organiser route pages are distinguished; historical GPX editions are described in notes or labels. Timed laps are not fixed race distances. Mixed timed/fixed weekends retain both types. Relay distance is the complete course, not each member's running distance.

Driving times/distances are coarse one-way road planning estimates from central Prague, without stops or traffic. Directions links open the relevant town or race base, not a verified car park. Where the future start is unknown, no drive estimate is invented.

## Implementation

Static HTML/CSS/JavaScript; no build step, backend, tracking or API keys. Fonts from Google Fonts, with system fallbacks. Serve this directory over HTTP to preview (the data loads with `fetch`).

Published at https://matejmicek.github.io/trail-atlas/
