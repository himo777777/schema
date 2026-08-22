# Proofloop public validation pilot

Proofloop tests a create → invite → participate → share → remix loop, with an A/B test of **Prediction Mode** on the seeded `7-Day Morning Focus` challenge.

## Public pilot scope

- Static, mobile-first web prototype.
- No login, payments, prizes, or monetary betting.
- Proof Points are non-purchasable, non-transferable, and non-redeemable reputation points.
- Names, challenge text, proof notes, photos, prediction choices, emails, and point balances remain in local browser storage.
- Optional, consent-based aggregate analytics use CounterAPI event counters only.
- Control variant hides Prediction Mode on the pilot challenge; treatment variant displays it.
- The query parameters `?variant=control` and `?variant=prediction` force a variant for QA.
- `?debug=1` shows local events and shared aggregate pilot counters.

## Primary gates

| Funnel | Target |
|---|---:|
| Challenge view → join | ≥20% |
| Join → first check-in | ≥50% |
| Prediction view → prediction | ≥25% |
| Prediction → share | ≥10% |
| Prediction → join | ≥5% |
| Prediction → create/remix | ≥1.5% |
| Referral/organic share of visits | ≥25% |

## Important limitation

Creator-generated challenges are device-local in this build and cannot yet be opened from another device. The first creator cohort must therefore be onboarded concierge-style: their challenge is added to the static pilot before they distribute it. This avoids building a database before the viral mechanism is validated.
