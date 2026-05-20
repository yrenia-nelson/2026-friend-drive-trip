# AGENTS.md

## Agent Coordination

This repo is expected to be edited by coding agents. Codex is editing it, and Antigravity, Google's coding agent, may also edit it. Get along, bots.

Keep a running change log in `JOURNAL.md`. When making meaningful changes, add a short dated entry with:

- who/what made the change, if known
- what changed
- why it changed
- any follow-up or uncertainty

Before editing, check `git status` and preserve work from other agents or humans. Do not overwrite unrelated changes. If another agent's edit conflicts with yours, reconcile it in the files and note the decision in `JOURNAL.md`.

All agents should be aware of the local JSON dumps in `data/celebrity-shorex/`. They are not throwaway cache files; they are the main captured data source for shore excursion analysis, copy analysis, price comparisons, stock checks, and future itinerary recommendations. Prefer reading these local JSON files before re-scraping or re-querying Celebrity.

## Celebrity Cruises API Notes

The shore excursion data in `data/celebrity-shorex/` came from the authenticated Celebrity Cruises Cruise Planner web app for the July 24, 2026 Celebrity Edge sailing.

Useful page:

- `https://www.celebritycruises.com/account/cruise-planner/category/shorex?bookingId=9346897&shipCode=EG&sailDate=20260724`

The app loads product data from:

- GraphQL: `https://aws-prd.api.rccl.com/en/celebrity/web/graphql`
- Promotions: `https://aws-prd.api.rccl.com/en/celebrity/web/commerce-api/catalog/v2/promotions/list?sailingId=EG20260724&page=plp&categoryId=shorex&currencyIso=USD`

The main GraphQL operations observed were:

- `WebCategoryAndFiltersById`
- `WebProductsByCategory`
- `WebProductByIds`

Important variables used by the Cruise Planner:

- `category`: `shorex`
- `shipCode`: `EG`
- `sailDate`: `2026-07-24` or `20260724`, depending on operation
- `reservationId`: `9346897`
- `regionCode`: `ALCAN`
- `currencyCode`: `USD`

The authenticated requests also require browser-session auth headers, including a bearer token and Celebrity/RCCL app headers. Do not commit those values. If fresh data is needed, capture requests from the logged-in browser or DevTools, use the token only transiently, and save only response JSON plus sanitized metadata.

The current capture includes:

- Paged product-list responses
- Combined product-list JSON
- Detailed product records for all captured excursions
- Promotions response
- Normalized copy-analysis inputs in JSON, JSONL, and CSV
- A markdown assessment report

Before committing newly downloaded data, run a secret scan such as:

```sh
rg -n "Bearer |authorization|appkey|eyJ0eXAi|access_token|refresh_token|account-id|vds-id" data/celebrity-shorex
```
