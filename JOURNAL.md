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

### Gold Creek Salmon Bake POI

- Antigravity documented the Gold Creek Salmon Bake as a Point of Interest (POI) under the Juneau cruise stop (July 27) and integrated it into the unbooked Dine & Sip Ideas table as a pescatarian-friendly port option.

### Excluded Helicopter Sled Dog Excursions

- Antigravity completely removed all helicopter-based glacier dog sledding options from both the daily schedules (July 27 and 28) and the independent comparison tables, focusing exclusively on ground-based, highly reliable Summer Musher Camps based on traveler preferences for safety, cost-efficiency, and reliability.

### Agent Coordination Convention

- Codex added this journal and updated `AGENTS.md` with agent coordination guidance.
- Purpose: keep future Codex / Antigravity / other-agent edits legible and reduce accidental overwrite or duplicated work.

### Road Trip Rebase for Brian, Kenny, Jhon, Julius, and Melanie

- Antigravity rebased the entire itinerary for a one-way, 12-day road trip from Hacienda Heights to Seattle for five friends (October 10-21, 2026).
- Removed all Celebrity cruise ports, shore excursions, and course compatibility tables since the group is doing a driving-only road trip and flying back.
- Created a brand-new "Outstanding Scenic Adventures & Local Rentals" table covering active outdoor rentals (e-bikes, railbikes, kayaking, paddleboarding) along the California-Oregon-Washington route.
- Rebuilt the master "Dine & Sip Ideas" directory with 24 premier dining spotlights along the highway route.
- Restructured the 3-track "Aligned Hotel Tracks" lodging guide for all 7 overnight hubs (Solvang, Santa Cruz, San Francisco, Fort Bragg, Crescent City, Portland, Seattle), including point-friendly and boutique recommendations for every stop.
- Restored the traditional `❓` (question mark) status indicator convention for all unbooked accommodations and recommendation tables, as requested by the user, keeping the interactive planning elements from the original template.
- Deleted the obsolete `data/celebrity-shorex` directory and all its cruise-specific JSON files.
- Overwrote `AGENTS.md` to remove cruise references and set new instructions for coding agents working on the rebased road trip workspace.

### Vancouver Trip Extension & Remote Repository Disconnection

- Antigravity integrated a two-day Vancouver, BC extension into the 12-day road trip schedule (October 19-20, 2026), followed by returning to Seattle for a departure flight back to Southern California on October 21.
- Updated all itinerary components with customized Vancouver details:
  - Added Day 9 (Seattle to Vancouver, BC) and Day 10 (Vancouver to Seattle) daily schedule blocks, complete with passport/Peace Arch warnings, e-bike and suspension bridge activities, public market food spotlights, and custom Google Maps route links with realistic border crossing buffer times.
  - Expanded the "Outstanding Scenic Adventures & Local Rentals" table with Stanley Park Seawall cycling options in Vancouver.
  - Expanded the "Master Dine & Sip Ideas" directory with Miku Vancouver and The Acorn.
  - Added premier Vancouver hotels and customized multi-night Seattle/Vancouver lodging schedules to the Boutique, Hilton Honors, and Marriott Bonvoy lodging tracks.
- Disconnected the legacy `cruise-origin` remote pointing to `yrenia-nelson/2026-cruise-drive-trip` to eliminate any risk of accidentally overwriting or clobbering the parallel cruise repository.
- Rebased `README.md` to cleanly align with the driving-only, 12-day friends' road trip workspace.

### Winery, Fishing, Dietary, Mapping, and Hotel Cost Updates

- Codex updated the main itinerary after user feedback that the group does not care about bike-focused activities and is instead interested in Napa/SLO wineries and fishing opportunities.
- Replaced the active rental/bike-heavy guide with a wineries and fishing opportunities section covering Santa Ynez/SLO/Paso/Napa tasting options plus Fort Bragg, Crescent City, and Seattle fishing leads.
- Added Melanie's pescatarian dietary restriction near the top of the itinerary and added a TODO for Google Antigravity to re-check all food and hotel options before booking.
- Added a rough full-trip Google Maps route link and a warning-tagged friends-review note for major decision points such as hotel minimum stays, wine detours, fishing-season uncertainty, and room-sharing comfort.
- Researched hotel costs across boutique, Hilton/points-friendly, and Marriott tracks using subagents and Chrome-backed rate checks where applicable. Updated the lodging section with 3-room minimum and 4-room comfort estimates that assume Mel has her own room and Kenny likely has his own room.
- Corrected the Crescent City points-friendly recommendation to Best Western Plus Northwoods Inn and noted that all hotel numbers are planning estimates requiring checkout verification.



