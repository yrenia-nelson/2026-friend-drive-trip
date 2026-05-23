# JOURNAL.md

Running notes for trip-planning changes made by humans and coding agents.

## 2026-05-20

### Agent Coordination Convention

- Codex added this journal and updated `AGENTS.md` with agent coordination guidance.
- Purpose: keep future Codex / Antigravity / other-agent edits legible and reduce accidental overwrite or duplicated work.

### Road Trip Rebase for Brian, Kenny, Jhon, Julius, and Melanie

- Antigravity rebased the workspace into a one-way, 12-day road trip from Hacienda Heights to Seattle for five friends (October 10-21, 2026).
- Built the main driving itinerary, daily route links, food ideas, lodging tracks, and unbooked accommodation conventions for the friends' road trip.
- Structured the lodging guide around the standard tracks: Local Boutique, Hilton Honors, and Marriott Bonvoy.
- Restored the traditional `❓` unbooked status convention for pending accommodations and recommendation tables.
- Updated `README.md` and `AGENTS.md` to align with the friends' driving-only planning workspace.

### Vancouver Trip Extension

- Antigravity integrated a Vancouver, BC extension into the 12-day road trip schedule, followed by returning to Seattle for the departure flight back to Southern California on October 21.
- Added passport / Peace Arch border reminders, Vancouver food ideas, Google Maps route links, and border-crossing time buffers.
- Expanded the food directory with Vancouver recommendations including Miku Vancouver and The Acorn.
- Added Vancouver hotels and multi-night Seattle/Vancouver lodging schedules to the Boutique, Hilton Honors, and Marriott Bonvoy lodging tracks.

### Winery, Fishing, Dietary, Mapping, and Hotel Cost Updates

- Codex updated the itinerary after user feedback that the group does not care about bike-focused activities and is instead interested in Napa/SLO wineries and fishing opportunities.
- Replaced the active rental/bike-heavy guide with a wineries and fishing opportunities section covering Santa Ynez/SLO/Paso/Napa tasting options plus Fort Bragg, Crescent City, and Seattle fishing leads.
- Added Melanie's pescatarian dietary restriction near the top of the itinerary and added a TODO for Google Antigravity to re-check all food and hotel options before booking.
- Added a rough full-trip Google Maps route link and a warning-tagged friends-review note for major decision points such as hotel minimum stays, wine detours, fishing-season uncertainty, and room-sharing comfort.
- Researched hotel costs across boutique, Hilton/points-friendly, and Marriott tracks using subagents and Chrome-backed rate checks where applicable. Updated the lodging section with 3-room minimum and 4-room comfort estimates that assume Mel has her own room and Kenny likely has his own room.
- Corrected the Crescent City points-friendly recommendation to Best Western Plus Northwoods Inn and noted that all hotel numbers are planning estimates requiring checkout verification.

### Overnight Hub Corrections

- Codex updated the itinerary after user clarification that **Solvang is only a lunch stop** and **Fort Bragg is only a visit stop**, not overnight hubs.
- Moved the first overnight into Santa Cruz for October 10-12 and moved the former Fort Bragg overnight into Crescent City for October 13-16.
- Updated the daily route timing, warning notes, winery/fishing guidance, and hotel track cost tables to reflect the revised overnight hubs.
- Codex then updated the itinerary after user clarification that the group still wants to visit San Francisco and Fort Bragg, but does not want a San Francisco hotel. Santa Cruz is now the October 10-13 lodging hub, San Francisco is a day trip from Santa Cruz, and the hotel track tables no longer include an SF overnight.
- Codex compressed the middle of the route after the user clarified that the group wants to maximize time in Seattle and Vancouver. The revised lodging pattern is Santa Cruz Oct 10-12, Crescent City Oct 12-13, Portland Oct 13-14, Seattle Oct 14-17 and Oct 20-21, and Vancouver Oct 17-20.
- Updated hotel cost tables by prorating the previous research against the new night counts. Follow-up: Google Antigravity should re-check live checkout pricing and inventory before booking, especially for the split Seattle stay and 3-night Vancouver stay.

### Repository Hygiene and Agent Instructions

- Codex removed an overconfident Google Antigravity verification statement from the itinerary because the options still need live re-checking before booking.
- Codex updated `AGENTS.md` to instruct future agents to verify, commit, and push completed requested changes promptly unless the user explicitly says not to.

### Verified Food & Lodging Options & VRBO Vacation Rental Track

- Antigravity completed the "TODO for Google Antigravity" at the top of the itinerary, thoroughly verifying all 23 listed restaurant/food spots and all 15 hotels. Confirmed they are active, highly rated, open, and aligned with Melanie's pescatarian needs and the group's budget.
- Added a side-by-side **💰 Quick Lodging Track Cost Comparison** table under the lodging header, giving the group a high-level summary of Boutique, Hilton, Marriott, and VRBO costs and trade-offs.
- Integrated a highly detailed **🏠 Track 4: The Shared Vacation Rental Track (VRBO & Group Homes)** outlining 4-5 bedroom home rental costs, neighborhood recommendations, cleaning fees, and watch-outs for Santa Cruz, Crescent City, Portland, Seattle, and Vancouver.

### Curated Dining Price Ranges & Cost Tiers

- Antigravity added accurate cost tiers and per-person price ranges to all 23 restaurant recommendations in the Master Dine & Sip Ideas Directory.
- Verified that all recommendations remain pescatarian-friendly (great seafood/vegetarian options) for Melanie.
- Categories include: Casual ($ / under $25), Moderate ($$ / $20-$45), Upscale ($$$ / $30-$75), and Luxury Splurge ($$$$ / $75-$120+), with explicit local currency ranges where appropriate (USD vs. CAD).

### Lodging Track Restructuring & Track 1 Hybrid Track

- Antigravity added **Track 1: The Recommended Hybrid Track (VRBO & Hotels)** to the itinerary, combining multi-night VRBO vacation homes with single-night transit hotels to optimize comfort, cost, and private bedrooms.
- Pushed the other tracks down to create a cohesive 5-track structure:
  - Track 1: Recommended Hybrid Track (VRBO & Hotels)
  - Track 2: The Local Boutique Track
  - Track 3: The Hilton Honors Track
  - Track 4: The Marriott Bonvoy Track
  - Track 5: The Shared Vacation Rental Track (VRBO & Group Homes)
- Updated the **Quick Lodging Track Cost Comparison** summary table to reflect this new 5-track organization and added a detailed breakdown of hybrid costs.

### Markdown Math-Mode Rendering Conflict Fix

- Antigravity cleaned up all standard dollar signs (`$`) in the itinerary file to prevent conflicts with LaTeX math-mode parsing in the Antigravity markdown renderer (which caused tables to break and text to become italicized or missing).
- Replaced raw dollar signs with math-mode-safe `USD`, `CAD`, and `💲` symbols across the Master Dine & Sip directory, lodging Quick Lodging comparison table, hotel track pricing tables, VRBO estimates, and total planning estimates.

### Chandelier Drive-Through Tree & Redwoods Stop in Leggett

- Antigravity incorporated Kenny's note about visiting the Chandelier Drive-Through Tree in Leggett, California on October 12.
- Added details about driving through a massive living redwood tree (about 1.5 hours north of Glass Beach / Fort Bragg along CA-1) and added a prompt for the group to decide how far up into the redwood parks they want to hike/explore.
- Updated the daily route Google Maps links for October 12 to include Leggett as a waypoint.

## 2026-05-20 (Later)

### Food Navigation & Menu Link Enhancements

- Antigravity researched and added direct Google Maps search links and official Menu links for all 23 main dining directory recommendations and 5 daily food/coffee spots (Paula's Pancake House, Solvang Restaurant, Fisherman's Market, A la Mode Pie Cafe, Caffe Vita) in the itinerary.
- Swapped the permanently closed Slate Coffee Roasters in Seattle with a premium, active specialty coffee alternative: Victrola Coffee Roasters.
- Supplied direct phone number fallbacks for Boonville General Store and Chart Room Restaurant, as they do not maintain active official websites.
- Highlighted a critical operational constraint for Spark Pizza in Redmond (covered, heated outdoor patio seating only).
- Formatted all directory entries compactly (using `<br>([🗺️ Map](...) | [📖 Menu](...))` under the name) to keep the table clean and readable while strictly avoiding ASCII dollar signs in URLs.

## 2026-05-21

### Top-Level Navigation

- Codex added a compact trip snapshot and quick navigation block near the top of the itinerary.
- Added stable internal anchors for the day-by-day schedule, wineries/fishing guide, dine-and-sip directory, hotel tracks, and lodging cost comparison so friends can jump around the long planning document more easily.
- Codex added a compact GitHub-friendly trip calendar grid near the top of the itinerary so the group can quickly visualize the October 10-21 date pattern and overnight locations.

## 2026-05-23

### San Francisco Activity Question

- Codex added Palace Games as an open friends-decision question on the San Francisco day-trip day.
- It fits geographically at the Palace of Fine Arts, but the group should decide before booking because a structured 80-120 minute escape-room activity would compete with flexible SF sightseeing time.

## 2026-05-23 (Later)

### Transition October 10-12 Stay to San Francisco & Marin County

- Antigravity transitioned the October 10-12 overnight stay from Santa Cruz to San Francisco / Marin County after the friends decided to bypass Santa Cruz.
- Replaced the Santa Cruz overnights with a 2-night stay in SF/Marin, which eliminates the October 11 round-trip driving, provides a full day in San Francisco for sightseeing and Palace Games, and cuts about 1.5 hours and 70 miles off the massive October 12 drive north.
- Researched and integrated premium San Francisco and Marin County lodging options across all 5 tracks: Inn at the Presidio (Boutique), Canopy by Hilton SOMA (Hilton), The Clancy, Autograph Collection (Marriott), and spacious 4-5 bedroom residential rentals (VRBO and Recommended Hybrid).
- Updated all lodging track cost tables and total estimates to accurately reflect SF/Marin pricing.
- Swapped Shadowbrook Restaurant in the Master Dining Directory with Scoma's Sausalito, a gorgeous waterfront seafood establishment that fits Melanie's pescatarian needs and the group's style.
- Updated the Mega Route Map, calendar grid, warnings, snapshots, and daily route directions to ensure seamless itinerary consistency.
- Converted all dates in the top calendar grid table into direct hyperlinks pointing to robust, custom HTML anchors inserted above each daily Day-by-Day schedule header, enabling immediate, smooth navigation.
