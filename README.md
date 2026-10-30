# Launch Truth — cards

Token launches checked against the chain. Every card line comes from public on-chain data and DexScreener, read at the time printed on the card. Facts, not financial advice.

- **Gallery:** `index.html`.
- **Cards:** `cards/<address>.svg`.
- **Receipts:** `receipts.json` (the data and method behind every line).
- **Corrections:** posted on X and in this repo's history.

## Card rules (the checks, and what changes a grade)

Each check is PASS, WATCH, FAIL or N/A, from public chain data and DexScreener only.

**Score:** (passes − 2 × fails) ÷ checks read.
- A ≥ 0.6
- B ≥ 0.3
- C ≥ 0
- D below 0
- F with 3 or more fails

**A requires no control risk,** so a token whose code one wallet can upgrade is capped at B.

| Check | PASS | WATCH | FAIL |
|---|---|---|---|
| supply | adds up across chains (< 0.01% off) | partial read / other supply model / < 0.5% off | ≥ 0.5% off |
| mint | no upgradeable mint path | one-wallet upgrade key | — |
| liquidity | ≥ $100k | ≥ $20k | < $20k |
| gap (cross-chain price) | ≤ 3% | ≤ 8% | > 8% |
| traction (24 h volume) | ≥ $50k | ≥ $5k | < $5k |
| survival | ≥ 72 h old and ≥ $10k/day | younger, or fading | volume faded |
| fees (tokenomics vault) | vault set | creator takes 100% / new hook not read | — |
| launch (launch-block buys) | < 3% of the pool | < 10% | ≥ 10% |
| team (platform token) | treasury steady over 7 d | treasury moved > 1M | — |
| burns (platform token, added 2026-10-30) | ≥ 5M burnt in 7 d | some burnt | none |

**Burns** is the core promise of a platform token (fees buy back and burn it). It applies to every platform token we card, whether it raises or lowers the grade. It was added before the first card was published.

## Disclosure

The operator holds $PANGEA. Cards follow the rules above whatever we hold, and every rule change is dated here.
