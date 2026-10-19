# Falsification Ledger

A public, append-only record of testable claims made about Bitcoin price models, with the pre-registered condition that would prove each one wrong and what happened when the date came due.

Maintained by [Colin Reed](https://modernwealthmodel.com) at Modern Wealth Model. The human-readable version, with sources and a changelog, lives at <https://modernwealthmodel.com/bitcoin-price-model-falsification-ledger/>. This repository holds the same data in machine-readable form.

## What is in `data/`

| File | What it is |
|---|---|
| `falsification-ledger.csv` / `.json` | One row per claim: 14 entries (7 pledges, 4 forecasts, 3 claims we could not verify). Each row has the claimant, the threshold, the dates, the resolution basis, a status, and a primary source. |
| `power-law-floor-watch.csv` / `.json` | A weekly series tracking Bitcoin's price against a power-law floor, using Newhedge as the named tracker. |

## Rules the data follows

- Rows are added when a claim is made and updated when it resolves. Entries are never deleted.
- The floor-watch series is append-only. A published row is not revised.
- Corrections are logged in the changelog on the page, not hidden.
- Nothing here predicts a price. The ledger records what others said and whether it held.
- A claim can appear under more than one status where it did both (for example, missed and not honored), so status counts are not additive.

## Using the data

The data is licensed CC BY 4.0. Attribute it as "Colin Reed, Modern Wealth Model, Falsification Ledger" and link to the page above. `CITATION.cff` has the machine-readable citation.

This is a living dataset and may contain errors. If you find one, open an issue with a primary source.
