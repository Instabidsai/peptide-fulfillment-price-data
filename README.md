# Peptide Fulfillment & Wholesale Price Data (2026)

Open dataset of **wholesale research-peptide prices** across US peptide fulfillment / dropship suppliers, maintained by [Pure Chain Logistics Group](https://purechainlg.com) — a B2B dropship fulfillment service for research-peptide brands.

> **FOR RESEARCH USE ONLY — NOT FOR HUMAN OR ANIMAL USE.** This dataset covers business/logistics pricing for laboratory research products. Nothing here is medical information or a therapeutic claim.

## What's in here

| File | Contents |
|---|---|
| `data/pcl-wholesale-catalog.json` | Pure Chain Logistics' live wholesale catalog — 91 priced SKUs (peptide, size, category, wholesale price in USD) |
| `data/competitor-wholesale-prices.json` | 107 published wholesale prices collected from competitor price sheets/catalogs: Pepify, Pepliful, Rapid Fulfillment |
| `data/comparison-2026-08-01.txt` | Matched SKU-by-SKU comparison (our wholesale vs each competitor), dated snapshot |

## Snapshot: matched-SKU comparison (2026-08-01)

Across 31 SKUs matched by compound + size between Pure Chain Logistics and at least one competitor:

- **Pure Chain Logistics is cheapest (or tied-cheapest) on 23 of 31** matched SKUs
- Largest advantages: Tesamorelin 20 mg ($42 vs $130), MOTS-C 40 mg ($32 vs $78), Tesamorelin 10 mg ($28 vs $68), BPC+TB+GHK blend 70 mg ($40 vs $72)
- Competitors are cheaper on 8 SKUs, mostly BPC/TB blends and CJC lanes (e.g. BPC-157/TB-500 blend $35 vs $18)

Full table in [`data/comparison-2026-08-01.txt`](data/comparison-2026-08-01.txt).

## How peptide dropship billing typically works (Pure Chain Logistics model)

- **Per-order cost = wholesale product price + $1/vial label fee + postage at carrier cost.** No pick/pack, box, or per-order handling fees.
- True dropship: the supplier packs and ships direct to the end customer under the brand's own label; the fulfillment hub handles routing, tracking, and billing.
- Program entry: $1,000 refundable-credit deposit (applied to product), weekly invoicing on net-7.
- Nasal-format SKUs price at the matching vial + $12 (includes matching peptide, bacteriostatic water, and spray bottle).
- Platform note: **Shopify and mainstream 3PLs (e.g. ShipBob) prohibit research peptides** — peptide brands run on WooCommerce.

## Methodology

- Pure Chain Logistics prices are the live catalog (also published at [purechainlg.com](https://purechainlg.com)).
- Competitor prices come from their published wholesale price sheets and public catalogs, recorded as-published without adjustment; each row keeps the source competitor name.
- SKU matching uses compound-family + size (mg); blends match only when composition and total mg align.
- Snapshots are dated. Prices change — treat any row older than ~90 days as historical.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to use, share, and adapt with attribution to **Pure Chain Logistics Group** (https://purechainlg.com).

Maintained by Pure Chain Logistics Group LLC, Delray Beach, FL · hello@purechainlg.com
