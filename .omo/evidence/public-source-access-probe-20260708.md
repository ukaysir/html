# Public source access probe

Generated: 2026-07-08T01:10:01+09:00

Method: agent-only public-source access probe. No login, phone, email, paid access, service-key use, or bypass attempted.

## Outputs
- data/public-source-access-probe-20260708.json
- source-access-map.html

## Results
| Source id | HTTP | Access class | Signals |
| --- | ---: | --- | --- |
| mcst_region_festival_download | 200 | public_page_download_or_file_hint | login_hint, download_hint, api_hint, javascript_hint, search_hint |
| data_go_kr_festival_standard | 200 | catalog_accessible_key_likely_required | service_key_hint, login_hint, download_hint, api_hint, javascript_hint, search_hint |
| data_go_kr_mcst_file | 200 | public_page_download_or_file_hint | login_hint, download_hint, api_hint, javascript_hint, search_hint |
| kto_datalab_festival | 200 | public_page_download_or_file_hint | login_hint, download_hint, api_hint, javascript_hint, search_hint |
| local_finance_cost | 200 | catalog_accessible_key_likely_required | service_key_hint, login_hint, download_hint, api_hint, javascript_hint, search_hint |
| local_finance_budget | 200 | catalog_accessible_key_likely_required | service_key_hint, login_hint, download_hint, api_hint, javascript_hint, search_hint |
| local_contract_status | 200 | catalog_accessible_key_likely_required | service_key_hint, login_hint, download_hint, api_hint, javascript_hint, search_hint |
| nara_bid_notice | 200 | catalog_accessible_key_likely_required | service_key_hint, login_hint, download_hint, api_hint, javascript_hint, search_hint |
| g2b_portal | 200 | public_page_accessible_probe_needed |  |
| lofin_portal | 200 | public_page_download_or_file_hint | login_hint, download_hint, javascript_hint, search_hint |

## Collection judgement
- Do not rely on generic web search alone. Use official catalog URLs, direct download pattern extraction, public portal search, and per-source access classification.
- For OpenAPI sources that indicate service-key use, record them as structured access constraints rather than attempting unauthorized collection.
- For JS-heavy portals, use public page/parameter observation only unless a documented public endpoint is visible.
