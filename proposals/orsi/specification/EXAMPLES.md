# ORSi Spec — illustrative commercial examples (active draft ORSi-01)

**Status:** Discussion examples; not mandated tariffs, protocol encodings, legal advice or implementation tests.

All customer-facing plan figures are hypothetical. Real pricing, refunds and data-retention rules belong to each provider's published contract. Billing should use the precise meter policy accepted by the customer.

## A. Prepaid voice AI on a USB device

- Device: a portable USB device with a provider-scoped reference `device-A-for-P1` (illustrative text, not a secure credential).
- Provider/service: `P1 / conversational-assistant`.
- Plan: **120 active talk minutes** in a separately offered time-denominated package, valid for **30 days** from a specified UTC activation time. This is not a general credit exchange.
- Meter: begins and pauses according to P1's published talk-time policy; the device merely being plugged in is not billed.
- Rule: if balance reaches zero first, service stops or requests an authorized top-up. If the validity window closes first, access stops even if unused minutes remain, subject to published carryover/refund policy.
- Audit: each billable period has a unique provider-owned receipt reference and corrections must be distinguishable from new usage.

## B. Postpaid specialist inference with offline operation

- Provider/service: `P2 / industry-inference`, independent of P1.
- Plan: usage-based monthly invoice with a contractual spending ceiling; the provider discloses the unit and rate.
- Challenge: the device is offline for a week, so the server may not know every event immediately.
- Rule: offline credit/exposure limits, reconciliation deadline and service behavior on unresolved evidence must be disclosed. The spec cannot promise perfect offline integrity on software-only storage.

## C. Monthly AI service subscription

- Provider/service: `P3 / voice-productivity`.
- Plan: monthly renewal with **600 included talk minutes** under a time-denominated offer, or a separately metered credit subscription; overage only if explicitly accepted.
- Rule: at period end, the plan follows its declared rollover, reset, nonpayment grace and cancellation policies. An unlimited label is not a license for undisclosed throttling or silent charges.

## D. One physical device, three providers

The same customer may use A (prepaid voice), B (postpaid specialist AI) and C (subscription) on one device. Each provider maintains its own entitlement, balances, receipts and customer agreement. A payment failure at B should not automatically revoke A or C. A shared market operator is optional, not required.

## E. Free/open service

A developer may offer a free local model under its own license or no monetary fee. ORSi Spec must not turn compatibility into a compulsory payment obligation. Usage restrictions, if any, should still be described honestly.

## F. Variable credits and talk-time benefits (hypothetical)

| Conversation example | Duration observed | Credits consumed | Potential charging basis |
| --- | --- | --- | --- |
| Efficient edge assistant | 14 minutes | 0.5 P1 credits | Low inference-resource consumption |
| Specialized cloud task | 4 minutes | 2 P1 credits | Higher-cost model tier |
| Optimized model workflow | 7 minutes | 0.3 P1 credits | Reduced compute demand |

All numbers are invented illustrations, **not measured performance, actual prices or quality rankings**. More conversational time or greater customer-perceived value can accompany lower credit consumption, but longer sessions are not intrinsically better. The provider must disclose a charge basis and a pre-agreed budget/cap or explicit authorization. There is no guaranteed number of minutes per credit. Separately purchased fixed-minute offers are permitted, but do not define a general credit exchange.

## G. Independent edge and shared cloud usage

The device runs a local model on an edge AI box and can separately connect to paid remote cloud inference. A hybrid mode switching to remote inference discloses data sharing, connectivity, provider identity and any change to metering before charges apply.

## H. Mobile-style recharge, maintenance, upgrade

After using part of an allowance, the customer recharges P1. P1 publishes whether the addition extends validity or creates a new credit bucket. A later model upgrade retains valid entitlements according to disclosed conditions and does not alter P2's separate balance.

## I. Two independently chosen provider models

**Direct inference company P4:** The customer purchases P4 credits under P4's resource/model-tier policy. A 3-minute hard task may consume more credits than a 15-minute easy conversation. P4 is the billing party; device vendors cannot rewrite its prices.

**OperatoR System provider P5:** P5 offers an authorized bundle of local model service and P4 inference. P5 may independently sell a prepaid subscription or credit package to the customer, subject to its supplier contract. P4's wholesale consumption and P5's customer price are distinct. They are not required to share credit denominations or talk-minute ratios.

Both offers may coexist on the same device. Actual charging choices, customer rights and limits remain under each provider's agreement.

## J. Hardware identity carrier versus inference execution

A USB device carries a signed entitlement reference but a separately attached laptop or edge AI box performs local inference. The physical USB device may contain model files, configuration, access rights or none of those beyond an identity reference. ORSi-01 does not assume the pendrive itself contains compute hardware. If a provider offers cloud fallback, it declares the actual inference provider, billing changes and privacy obligations.

## K. Three independent commercial quantities

A hypothetical plan may expire on a given date, retain a provider-defined credit balance and separately count purchased active-use hours; measured conversation duration is an optional fourth reported quantity. Adding 10 credits does not necessarily change the expiration date or extend active-use hours. Extending validity does not refill spent credits. The exact offered combination and carryover rules are provider-owned and customer-accepted.

## L. Reuse-first automation with optional alerts and no hard cap

An operator has a previously reviewed routine for checking system state, applying an approved change only when needed, and verifying the result. On repeated compatible requests, the routine performs the deterministic work locally; where the state is already correct, it reports completion without invoking the model again. Inference might be used only for a changed requirement or uncertain result.

Under a **remote-inference-based plan**, fewer fresh inference calls can mean fewer such usage charges. Under a **runtime-hours or subscription plan**, the contract may still bill for authorized operation. No universal promise of zero cost follows from reuse.

The customer chooses an **alerts-only plan** with illustrative notifications at 50 and 100 provider-defined billing units but no automatic stop. A different customer chooses a **hard spending ceiling** that pauses additional billable work; a third explicitly authorizes **uncapped** postpaid operation after seeing the charging rules and provider limits. All are valid ORSi offerings if accepted by the respective provider and customer. If alerts cannot be delivered during offline work, the contract discloses that limitation. Neither alerts nor uncapped operation bypasses entitlement expiry or legitimately enforced provider restrictions.

## M. Three-party offer: known workflow and genuine inference

**User:** Under a valid, properly described "unlimited workflow access" plan, the same approved task can be performed repeatedly without an ORSi-imposed invocation count. An authorized deterministic routine executes known work and verifies the output, possibly requiring **zero fresh model calls**.

**Inference company:** If a novel request later requires cloud inference, the supplier provides and bills that **actual inference** under its own credits, validity and commercial terms. No billable supplier inference event should be asserted when the supplier did not provide one. The supplier may still have separately contracted capacity, software or subscription fees.

**AI service provider:** The operator sells a supported service that combines reusable approved workflows with appropriately licensed model access and genuine on-demand inference. Lower repeated-task inference use can improve service economics while subscriptions, support and licensed runtime charges remain governed by the customer agreement.

The customer may separately select an authorized uncapped postpaid plan, alerts-only control, or a spending cap. Unlimited workflow access is **not** itself consent to unlimited postpaid debt, unlimited remote inference, or access after expiry.

## N. Telecom-style single-device unlimited plan (hypothetical)

**Device D:** One enrolled USB AI key, whose permitted inference execution can occur on a separately supported host computer. Device identity is not presumed to be cryptographically authenticated merely from its public serial.

**Provider P1:** Offers a 30-day plan with unlimited repetitions of **included, approved local workflows for Device D**. A familiar status-check routine may repeat without fresh model calls. The plan does not automatically cover a second device, unapproved tasks, or service after the published expiry. P1 may separately authorize rebind or extra devices under its terms.

**Inference provider P2:** Independently supplies premium cloud inference to the same Device D under P2's own credits or subscription. P1's 'unlimited' local workflow plan does not make P2's cloud calls free, alter P2's balance, or force a fixed credit/minute exchange.

**Customer choice:** Another provider might offer fixed-minute conversation bundles, uncapped postpaid access, alerts-only service, a per-inference charge, or a multi-device plan. ORSi does not require every provider to sell the P1 model. Any fair-use/availability conditions must be disclosed, and a plan's unlimited task repetitions do not constitute consent to unlimited postpaid spending.

## What these examples do not establish

They do not establish cryptographic hardware proof, trusted offline clocks, rollback-proof state, hard availability guarantees or verified legal enforceability.
