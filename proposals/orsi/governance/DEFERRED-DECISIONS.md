# ORSi Spec — Deferred decisions register

**Preparation only · 2026-11-18.** These are **not** defaults or promises; future business cases and stakeholder review may resolve them.

| ID | Decision | Preparation treatment |
| --- | --- | --- |
| DD01 | Universal credits-to-talk-time conversion or mandated tariff | **NOT_APPLICABLE** — no universal exchange or price |
| DD02 | Unlimited device plan's included routines, validity, fair-use, price | **PROVIDER_DEFINED** — clearly disclose in a real offer |
| DD03 | Recharge, carryover, expiry, refunds, active-use hours | **PROVIDER_DEFINED** — no invented balance or rollover rule |
| DD04 | Prepaid/postpaid/subscription unit, invoice cycle, alerts or authorized uncapped mode | **PROVIDER_DEFINED** — no required spending ceiling |
| DD05 | Device hardware authentication, trusted clock, offline balance freshness | **DEFERRED** technical profile — no false security assurance |
| DD06 | Credit transfer, account migration, one provider accepting another's wallet | **DEFERRED** — no automatic commercial portability |
| DD07 | Cloud inference fallback/consent, model/service versions | **PROVIDER_DEFINED** now; common interoperability details may be **DEFERRED** |
| DD08 | Model format, runtime SDK, billing transport, payment gateway | **OUT OF SCOPE** of the first commercial profile |
| DD09 | ORSi trademark clearance, contributor ownership, release steward | **OPEN PUBLICATION GATES** — cannot skip at release |

A `PROVIDER_DEFINED` value may remain undecided in prep, **but cannot stay hidden if a paid customer depends on it**. A `DEFERRED` standard feature does not magically exist. A `NOT_APPLICABLE` service feature should not be misrepresented as free, unlimited or guaranteed.

For evolving a bounded requirement, use [Progressive Policy](PROGRESSIVE-SPECIFICATION.md), separate non-normative telecom case studies and the preparation workstream's open questions (not part of this release package).
