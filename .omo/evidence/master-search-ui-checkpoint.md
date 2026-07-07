# Master search UI checkpoint

Date: 2026-07-08

Changed:
- The search panel now attempts to load `data/master/mcst-region-festivals-2017-2026.lite-index.json`.
- If loaded, searches include MCST 2017-2026 master draft rows as well as curated case cards.
- If opened as a local `file://` page and fetch is blocked, the existing curated case search still works.

Caveat:
- Search is client-side and capped to 60 displayed MCST rows per query for readability.
