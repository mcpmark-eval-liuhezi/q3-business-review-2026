# Q3 2026 Store Ops Digest

Prepared for the quarterly business review (moved up to Friday). All figures below are pulled live from the WooCommerce store, the Notion wiki, GitHub, and Weights & Biases on 2026-10-22.

## Starting catalog count

The live catalog contained **0 products** before the two Q3 announcement items were added. A full product list call (100 per page) and a targeted search both returned empty.

## Last month's sales figures (September 2026)

- Total sales: **$0.00**
- Net sales: **$0.00**
- Average sales: **$0.00**
- Total orders: **0**
- Total items sold: **0**
- Total tax: **$0.00**
- Total shipping: **$0.00**
- Total refunds: **0**
- Total discount: **$0.00**
- Total customers: **0**

Every day of the month (2026-09-01 through 2026-09-30) reported $0.00 sales and 0 orders.

## New SKUs announced at the review

| SKU | Product name | Regular price | Stock | Product ID | Status |
| --- | --- | --- | --- | --- | --- |
| Q3BR-GIFT | Q3 Review Gift Chest | $49.90 | 25 | 10 | Published / In stock |
| Q3BR-SAMPLE | Q3 Review Sample Pack | $19.90 | 40 | 11 | Published / In stock |

Both products manage stock explicitly and are visible in the catalog.

## Low-stock findings

The low-stock report endpoint (`/reports/stock/low`) is **not available on this store** - it returns "WooCommerce API endpoint not found", and the general stock report endpoint (`/reports/stock`) fails the same way. With an empty starting catalog, no stock thresholds were configured and no items were flagged as low or out of stock prior to the new SKUs. Neither new SKU carries a custom low-stock threshold, so nothing is currently flagged low.

## Internal test order

- Order number: **#12** (status: pending, created via REST API)
- Line items: 1x Q3 Review Gift Chest (Q3BR-GIFT, $49.90) + 1x Q3 Review Sample Pack (Q3BR-SAMPLE, $19.90)
- Order total: **$69.80**
- Internal note (not customer-facing): "Internal QBR prep order - not for shipment, logged for the quarterly review."

## Wiki search outcome (Notion)

The wiki contains QBR-related material, though no dedicated agenda for this Friday's review:

- **QBR Prep Notes - Orbit 4.2 Launch Review** (parent: QBR prep collection) - the only page with substantive QBR content. It contains final notes for a quarterly business review plus four agenda items: launch metrics walkthrough, customer escalation log, hiring update, and budget reallocation proposal.
- **Cobalt Energy QBR Prep**, **Bright Harbor QBR Prep**, **Atlas Logistics QBR Prep** - three QBR prep pages, all empty bodies.
- **Q3 Safety Audit Board Pack** - Q3-adjacent but about safety audit CAPA findings, not the store ops review.
- A search for "quarterly business review" returned unrelated pages (handover notes, stack review brief, access audits, art sessions, trip briefs).

## Pull request

This digest is committed on branch `digest/q3-2026-store-ops` and opened as a pull request titled "Add Q3 store ops digest" targeting the default branch (`main`). A comment review has been left on the digest file confirming the figures tie back to the store and the order is logged.
