# MCST download probe checkpoint

Date: 2026-07-08

Result:
- HEAD requests to the annual ZIP endpoint returned 403 for 2017-2026.
- GET requests succeeded for every year from 2017 through 2026.
- Byte sizes and SHA-256 hashes are recorded in `data/mcst-download-probe.json`.

Raw files:
- Downloaded only to the local temp directory during the probe.
- Not committed to the repository.

Next:
- Extract the downloaded ZIPs in a temporary workspace.
- Identify file types and schemas.
- Commit derived normalized JSON/CSV records, not opaque binary ZIPs, unless raw-file archival is explicitly desired.
