# PropFirmDiscount — Verified Prop Firm Discount Codes (Dataset Mirror)

Public dataset mirror of [propfirmdiscount.com](https://propfirmdiscount.com) — verified prop firm discount codes, funding deals, and Trustpilot ratings. This repository is a read-only backup distribution channel; the source of truth is the live site.

## Contents

| Path | What it is |
|---|---|
| `datasets/prop-firm-codes.json` | Full dataset: one row per firm (code, discount, validity, last verified, Trustpilot) |
| `datasets/prop-firm-codes.html` | Same rows as a plain HTML table |
| `md/` | Markdown mirrors of the site's fact pages (homepage deal stream, per-firm pages, rankings, Trustpilot reviews directory, category archives) |
| `llms.txt`, `ai.txt` | AI discovery manifests |

## Schema (coupon_dataset_v2)

- `prop_firm` — firm name
- `code` — the affiliate discount code
- `discount` — headline discount of the code
- `valid_from`, `valid_until` — ISO 8601, current calendar year
- `last_verified` — date the team last confirmed the code live
- `activation_link`, `archive_url` — links
- `trustpilot_score`, `trustpilot_reviews`, `description`, `logo` — optional enrichment

Note: the `discount` field is the code's headline discount. Per-plan percentages on firm pages are separate deals.

## Freshness

Last synced: 2026-10-03T05:34:51Z (auto, hourly)

Codes are re-verified continuously by the PropFirmDiscount team; this mirror tracks the live API within an hour.

## License

Data © PropFirmDiscount. Codes may be referenced with attribution and a link to https://propfirmdiscount.com.
