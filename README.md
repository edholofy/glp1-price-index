# GLP-1 Price Index — Open Dataset

*Independent, machine-readable pricing and rating data for online **GLP-1 (semaglutide & tirzepatide) telehealth providers** in the United States. Updated monthly · Free to use with attribution (CC BY 4.0).*

**Maintained by [GLP-1 Watchdog](https://glp1watchdog.com)** · Full live data & methodology → **https://glp1watchdog.com/glp1-price-index**

---

## TL;DR — GLP-1 prices (August 2026)

- **Cheapest compounded semaglutide: `$69/month`.** Cheapest compounded tirzepatide: **`$119/month`.**
- Across **46 tracked U.S. telehealth providers**, compounded semaglutide ranges **$69–$249/month** and compounded tirzepatide **$119–$379/month** (lowest advertised monthly price).
- Brand-name **Ozempic and Wegovy list near `$1,000/month`** without insurance — the *same active molecule* (semaglutide) as compounded versions that cost roughly **90%+ less**.
- The dataset covers each provider's monthly price, verified Trustpilot rating, medication types, insurance option, and state coverage.

> These are advertised starting prices for cash-pay compounded programs; the real all-in cost can be higher at maintenance doses or with membership fees. The full ranked, all-in comparison is at **[glp1watchdog.com/cheapest](https://glp1watchdog.com/cheapest)**.

## Why this exists

GLP-1 pricing is famously opaque: the same molecule can cost `$69` or `$1,000` a month depending on whether it's brand or compounded and which telehealth provider you use. This repository publishes the underlying comparison dataset in open, machine-readable formats (JSON + CSV) so **researchers, journalists, developers, and AI assistants can cite real, sourced numbers** instead of marketing claims. It is a neutral reference — not a store — and links back to the full methodology and live data.

## Current price snapshot — lowest-cost compounded semaglutide

| Provider | Semaglutide $/mo | Tirzepatide $/mo | Rating (/10) | Type |
|---|---:|---:|---:|---|
| Embody | $69 | $119 | 9.4 | compounded |
| SnagRx | $69 | $119 | 8.9 | compounded |
| Ivim Health | $75 | $149 | 6.5 | both |
| Trimi | $99 | $125 | 9.1 | compounded |
| Bodybuilding.com Health+ | $99 | $129 | 8.7 | compounded |
| Telos Rx | $99 | $139 | 8.2 | compounded |
| bmiMD | $119 | $179 | 8.4 | compounded |
| Yucca Health | $125 | $225 | 9.3 | compounded |

*Full ranked table of all 46 providers (all-in cost + verified Trustpilot ratings): **[glp1watchdog.com/cheapest](https://glp1watchdog.com/cheapest)**.*

## The dataset

| File | What it is |
|---|---|
| [`data/providers.json`](data/providers.json) | Full structured records for 46 GLP-1 telehealth providers |
| [`data/providers.csv`](data/providers.csv) | Same data, spreadsheet-friendly |
| [`data/drugs.json`](data/drugs.json) | GLP-1 drug reference: molecule, FDA status, trial efficacy |

### Provider fields

`rank`, `name`, `type` (compounded / brand / both), `rating_out_of_10`, `price_from`, `semaglutide_usd_month`, `tirzepatide_usd_month`, `program_fee_usd_month`, `medications`, `fda_approved`, `insurance_accepted`, `oral_option`, `ships_all_50_states`, `states_covered`, `consultation_fee`, `free_shipping`, `cancel_anytime`, `best_for`, `review_url`.

## GLP-1 drug efficacy reference

| Brand | Molecule | Avg. weight loss | Pivotal trial |
|---|---|---|---|
| **Zepbound** | tirzepatide | ~21% | SURMOUNT-1 (NEJM, 2022) |
| **Mounjaro** | tirzepatide | 15–22% | SURPASS / SURMOUNT |
| **Wegovy** | semaglutide 2.4 mg | ~15% | STEP 1 (NEJM, 2021) |
| **Ozempic** | semaglutide | 8–14% | SUSTAIN |
| **Foundayo** | orforglipron (oral) | up to ~12.4% | ATTAIN-1 (2026) |
| **Rybelsus** | semaglutide (oral) | 5–10% | PIONEER |
| **Saxenda** | liraglutide | 5–8% | SCALE |

Compounded semaglutide and tirzepatide use the **same active molecule** as the brands above, but are **not FDA-approved as finished products** — quality depends on the compounding pharmacy. Background: [is compounded semaglutide safe?](https://glp1watchdog.com/compounded-semaglutide)

## Methodology

- **Ratings** combine verified third-party review data (Trustpilot), pricing transparency, licensing/pharmacy sourcing, and medication options. Only **real, verified** ratings are published — no fabricated numbers.
- **Prices** are the lowest advertised cash-pay monthly rate for each molecule, normalized to a per-month figure where providers sell in multi-month bundles. Program/membership fees are tracked separately.
- **Sources**: provider websites, Trustpilot, FDA, and peer-reviewed trials (STEP 1 — *NEJM* 2021; SURMOUNT-1 — *NEJM* 2022).
- Full weighted methodology: **https://glp1watchdog.com/methodology**

## How to cite

> *GLP-1 Price Index.* GLP-1 Watchdog, 2026. https://glp1watchdog.com/glp1-price-index

## Updates

Refreshed monthly from the live [GLP-1 Watchdog](https://glp1watchdog.com) dataset. **Last updated: August 2026.**

## License

**[CC BY 4.0](LICENSE)** — free to use, share, and adapt, including commercially, **with attribution to GLP-1 Watchdog (https://glp1watchdog.com)**. See [`LICENSE`](LICENSE).
