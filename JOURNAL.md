# JOURNAL.md

Running notes for trip-planning changes made by humans and coding agents.

## 2026-05-20

### Repo Setup and Initial Itinerary

- Codex copied the Pacific Northwest trip itinerary into this repo and committed it as `b808f8b Add Pacific Northwest trip itinerary`.
- The itinerary established the road trip to Seattle, Celebrity Edge cruise timing, hotel option tracks, and school/course compatibility notes.

### Celebrity Shore Excursion Data Capture

- Codex inspected the Celebrity Cruises Cruise Planner web app and identified the API path behind the shore excursion planner.
- Codex downloaded sanitized Celebrity shore excursion JSON into `data/celebrity-shorex/` and committed it as `44eb536 Add Celebrity shore excursion data`.
- Captured data includes product pages, combined product list JSON, detailed product records, promotions, normalized copy-analysis inputs, and the markdown shore excursion assessment.
- All agents should treat the JSON dumps in `data/celebrity-shorex/` as important local source data, not disposable generated output. Use them before re-querying Celebrity.
- Important safety note: auth tokens and request headers were intentionally not committed.

### Agent-Facing Repo Notes

- Codex added `README.md` and `AGENTS.md` in `e254116 Add agent notes and e-bike interest`.
- `README.md` explains that this repo is meant to be used with coding agents such as Codex, Antigravity, and similar tools.
- `AGENTS.md` records the Celebrity API discovery notes and the secret-scan rule for future data refreshes.

### E-Bike and Unbooked Planning Notes

- Codex added an unpurchased Victoria e-bike interest note for Nelson and Yrenia in the main itinerary.
- Codex added independent e-bike alternatives for Ketchikan, Juneau, Skagway, and Victoria in `d86383a Update itinerary planning notes`.
- Codex marked hotels and dinner ideas as unbooked with the `❓` convention.
- Codex updated the traveler logistics note: Nelson and Yrenia road-trip to Seattle; Mom and Brother fly into Seattle and join for the cruise.

### Subsequent Itinerary Refinements

- Another agent or human added pescatarian-friendly dinner ideas and Yrenia's mushroom preferences in `1f0e423 Flesh out itinerary with pescatarian-friendly dining ideas and Yrenia's mushroom preferences`.
- Another agent or human updated and verified independent e-bike alternatives with dock alignments and cleaner URLs in `30819f4 Update and verify independent e-bike alternatives with dock alignments and clean URLs`.
- Another agent or human fixed markdown strikethrough rendering by replacing unescaped tildes in `0509568 Fix strikethrough rendering bug by replacing unescaped tildes with approx. and about`.

### Sled Dog Activity Research and Comparison

- Antigravity researched Juneau and Skagway dog sledding excursions from the Celebrity catalog and compared them to independent booking options.
- Added a comprehensive `Independent Sled Dog Alternatives to Compare` table in the main itinerary and documented these options as unpurchased interest bullet points under Juneau (July 27) and Skagway (July 28) in the daily cruise stops.
- Highlighted the critical distinction that Skagway's glacier helicopter tour is a **demonstration only** (no guest rides), whereas Juneau's glacier tour includes an actual mushing ride on snow.
- Documented land-based summer musher camps (wheeled carts) in Juneau and Skagway as highly reliable, more affordable alternatives that aren't subject to weather cancellations.

### Real-World Travel Time Modeling

- Antigravity updated the driving legs throughout the itinerary to explicitly distinguish between "pure driving time" and "total elapsed travel time" (including realistic buffers for lunch, dinners, stretch breaks, and fuel stops).
- Adjusted arrival times to match the realistic modeling, ensuring the travelers have accurate time expectations for their road segments.

### Agent Coordination Convention

- Codex added this journal and updated `AGENTS.md` with agent coordination guidance.
- Purpose: keep future Codex / Antigravity / other-agent edits legible and reduce accidental overwrite or duplicated work.
