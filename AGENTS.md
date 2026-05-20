# AGENTS.md

## Agent Coordination

This repo is expected to be edited by coding agents. Codex is editing it, and Antigravity, Google's coding agent, may also edit it. Get along, bots.

Keep a running change log in `JOURNAL.md`. When making meaningful changes, add a short dated entry with:

- who/what made the change, if known
- what changed
- why it changed
- any follow-up or uncertainty

Before editing, check `git status` and preserve work from other agents or humans. Do not overwrite unrelated changes. If another agent's edit conflicts with yours, reconcile it in the files and note the decision in `JOURNAL.md`.

## Road Trip Planning Workspace

This repository has been fully rebased as a planning workspace for the **2026 Coastal California & Pacific Northwest Road Trip** for five friends (Brian, Kenny, Jhon, Julius, and Melanie), traveling from October 10–21, 2026.

All previous cruise-specific materials, API integrations, and associated shore excursion JSON caches have been deleted as they are completely irrelevant to this driving-only trip.

### Guidelines for Editing the Itinerary:
- **Itinerary File:** The main trip document is [Pacific Northwest Trip Itinerary.md](file:///Users/nelson/code/2026-friend-drive-trip/Pacific%20Northwest%20Trip%20Itinerary.md).
- **Accommodation Status:** Keep the `❓ *Unbooked*` convention on accommodation lines for daily schedules to represent pending reservations. E.g., `* **Accommodation:** ❓ *Unbooked* in [Location] (See hotel tracks below).`
- **Loyalty & Style Alignment:** Keep hotel recommendations organized into the three standard tracks: *The Local Boutique Track*, *The Hilton Honors Track*, and *The Marriott Bonvoy Track*.
- **Maps Links:** All daily routes must feature direct Google Maps links modeled using the standard `https://www.google.com/maps/dir/?api=1&origin=...&destination=...&travelmode=driving` format.
- **Realistic Time Modeling:** Always distinguish between "pure driving time" and "total elapsed travel time" (including food, gas, and stretch breaks) to maintain realistic travel expectations.
