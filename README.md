# Kitfinch verified small-business software prices

Open dataset of list prices for business software used by US small service businesses (field service, phones, payroll, scheduling, POS, CRM and more). Every row was checked on the vendor's own pricing page, is dated, and links back to that page.

- **Rows:** 132 plans across 45 tools
- **Last verified:** 2026-10-05
- **License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- **Live version:** [kitfinch.com/data](https://kitfinch.com/data) (this repository is a snapshot)

## Files

| File | Format |
|---|---|
| `prices.csv` | One row per plan |
| `prices.json` | Same rows, with dataset metadata (`name`, `license`, `attribution`, `lastVerified`, `count`) |

## Columns

| Column | Meaning |
|---|---|
| `tool` | Tool slug, as used in kitfinch.com URLs |
| `tool_name` | Display name |
| `plan` | Plan name as written by the vendor |
| `amount_usd` | Price in US dollars |
| `period` | `month` (flat per account), `user_month` (per user per month) or `report` (per report) |
| `billing` | `annual`, `monthly` or `standard` (the vendor shows a single price) |
| `min_units` | Minimum seats or units the vendor requires, when stated |
| `verified_at` | When the price was read on the vendor page (UTC) |
| `source_url` | The vendor page the price came from |
| `kitfinch_url` | The Kitfinch pricing page for that tool |

## How prices are checked

Prices are read on the vendor's public pricing page and stored with the date and the source URL. A price that cannot be tied to a public vendor page is not published. The full method is on [kitfinch.com/methodology](https://kitfinch.com/methodology).

Prices change. Always confirm on the vendor page before buying, and open an issue if you spot an outdated row.

## Attribution

Please credit: **Kitfinch (https://kitfinch.com/data)**

## About Kitfinch

[Kitfinch](https://kitfinch.com) ranks business software by trade for US small service businesses: plumbers, HVAC contractors, salons, dentists, restaurants and more. Contact: contact@kitfinch.com
