# ORSi Spec — Progressive specification policy

**Owner direction R09 · Preparation draft · 2026-11-18.** Do not freeze every business model at once. ORSi's first profile should provide *shared commercial meanings*, while individual inference companies and OperatoR System providers define their own offerings.

## Decision statuses

| Label | Meaning |
| --- | --- |
| **COMMON_CANDIDATE** | Minimum interoperability concepts to propose for review: provider/issuer, service, enrolled device and plan scope, access status, applicable validity and reference to customer terms |
| **PROVIDER_DEFINED** | Provider chooses the price, credit meter, included unlimited routine list, expiry, recharge, paid support, alerts, refund and fair-use rules |
| **DEFERRED** | No ORSi-wide decision; wait for a concrete customer/provider need and an independently reviewed proposal |
| **NOT_APPLICABLE** | Feature is not sold or used in the offer, such as talk-time charging in a task-priced plan |

These are **draft editorial labels**, not a wire format, official conformance status or certification.

## What should be common now?

A device-associated entitlement should explain who offers and bills, which service and device/scope it covers, whether it is active, its actual access/validity terms, and how a customer finds the applicable commercial contract. Device identification is not proof of hardware authenticity. Different providers can coexist without shared billing control.

Provider credits, observed conversation time, active-use hours, calendar validity and inference resource use are independent. ORSi sets **no credit-to-minute conversion, global tariff, mandatory single-device unlimited plan or required spending cap**.

## Blank during drafting is not blank at purchase

The **spec draft** may mark a feature `PROVIDER_DEFINED`, `DEFERRED` or `NOT_APPLICABLE`. But **an actual paid offer** cannot silently omit material price, expiry, covered activity, billing responsibility or restrictions. Missing validity must not be interpreted as perpetual access; missing credits cannot imply zero cost; an unidentified USB serial cannot imply cryptographic security.

## Business-driven expansion

When a provider has a new use case, document its actual problem, parties, optional versus universal scope, customer transparency, privacy and security assumptions, scenarios, backwards compatibility and reviewer conclusion. Define only the smallest new piece needed and preserve earlier drafts. Never convert one provider's tariff into an obligation for every provider.

References: separately maintained, non-normative telecom case studies, [Deferred decisions](DEFERRED-DECISIONS.md), and [Release process](RELEASE-PROCESS.md).

**Current state:** a parked candidate for future release; no code, hardware experiments, conformance tests or automatic publication. Formal adoption requires explicit review and approval.
