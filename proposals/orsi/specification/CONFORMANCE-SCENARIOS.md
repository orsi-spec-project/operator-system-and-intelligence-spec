# ORSi Spec — human-readable review scenarios (active draft ORSi-01)

**Status:** Proposed review checklist. **All scenarios: NOT_RUN / NOT_RATIFIED.** No implementation or conformance tests are included in this repo.

| ID | Scenario | Expected contract-level observation |
| --- | --- | --- |
| S01 | New prepaid entitlement on a known device reference | The customer can identify provider, service, validity, units, allowance and renewal rules |
| S02 | Optional time-metered plan spans multiple sessions | Only a purchased time plan charges minutes at its disclosed boundaries; ordinary talk-time reporting is not automatically billable |
| S03 | Prepaid allowance exhausted | Access changes in the published way; exhausted credit is not silently restored |
| S04 | Time-denominated entitlement expires with minutes remaining | Published expiry and rollover/refund terms govern; unused allowance not silently reclassified |
| S05 | Subscription renews successfully | New period and included allowance are disclosed; carryover follows published terms |
| S06 | Subscription payment fails | Declared grace, pause, overage prevention and cancellation rules apply |
| S07 | Postpaid customer-selected spending cap hit | When a hard cap was selected, further billable work follows the agreed pause/stop policy; reconciliation is traceable |
| S08 | Postpaid offline reporting delayed | Provider discloses offline ceiling, trust assumptions and reconciliation deadline |
| S09 | Duplicate/retried usage receipt | One billed event is not charged twice; adjustments remain auditable |
| S10 | Two providers share one physical device | A cannot debit, suspend or renew B's allowance by default |
| S11 | Hardware replaced or lost | Provider's disclosed rebind, refund and recovery rules apply |
| S12 | USB serial copied or software image cloned | Implementation must not claim unique physical authentication based solely on public metadata |
| S13 | Old local usage state restored | Software-only history cannot be claimed rollback-proof; uncertainty is handled per policy |
| S14 | Customer disputes billed usage or optional minutes | Customer can inspect provider, actual billed unit, charge periods and correction reference without disclosing conversation content by default |
| S15 | Fair-use or free service is selected | No mandatory ORSi platform tariff; provider states any legitimate restrictions |
| S16 | Service goes offline or shuts down | Contract defines service interruption, portability, exit and outstanding credit disposition |
| S17 | Another meter used instead of talk time | Unit is clearly identified; tokens, GPU-seconds and minutes are not silently substituted |
| S18 | Time zone or clock changes | UTC validity boundaries and trusted-time limitations are disclosed |
| S19 | Variable provider charging policy published | Unit, model/task tier, effective revision, limits and separate talk-time measure are disclosed, without a fixed credit/minute ratio |
| S20 | Two providers use unrelated credits | No cross-provider balance or conversion is implied |
| S21 | Device idle or session interrupted | Only provider-disclosed billable active usage is charged |
| S22 | Credit charging policy changes mid-session | Policy version, customer consent and applicable caps are traceable; settled use not repriced |
| S23 | Recharge after partial usage | Purchased balance is preserved under disclosed terms; spent balance not resurrected |
| S24 | Upgrade or device maintenance | Balance, access and version consequences are explained before changes |
| S25 | Edge inference falls back to cloud | Provider, consent, privacy, network and charge implications are disclosed |
| S26 | Provider A cancels while B stays active | Provider B's entitlement is not independently modified |
| S27 | Credit exhaustion during conversation | Stop, pause, recharge or authorized overage follows the accepted plan |
| S28 | Equal talk duration, unequal inference cost | Credits can differ according to disclosed resources/tasks; no fixed time conversion assumed |
| S29 | Efficient model gives more value for fewer credits | Credit use and talk-time benefit differ; no unsupported objective quality claims |
| S30 | Variable-cost request initiated | Customer knows charging basis and selected control: hard cap, alerts-only or explicitly authorized uncapped mode |
| S31 | Reserved credits exceed settled cost | Unspent credit reservation is released/reconciled and evidenced by receipt |
| S32 | Guaranteed-minute package coexists with variable credits | Time guarantee applies only to the purchased package |
| S33 | Direct inference provider offers credit plan | That provider controls the accepted charge basis; device vendor cannot reprice it |
| S34 | OperatoR System provider offers an authorized third-party bundle | Retail credits and upstream supplier settlement are separate and customer billing party is identifiable |
| S35 | Talk time reported under a resource-metered plan | Minutes do not intrinsically trigger credit debit |
| S36 | Different providers charge different credits for equal duration | Independent price/meter policies are valid and disclosed |
| S37 | USB carrier holds licence but external host runs inference | Service discloses the actual execution host, device dependency and offline requirements |
| S38 | Device removed or identity becomes uncertain during active usage | Provider follows declared pause/continuation/recovery policy; unsupported authentication claims are avoided |
| S39 | Customer recharges validity only or credits only | Each entitlement axis changes only as authorized; previously spent credit is not restored |
| S40 | Offline usage evidence is uncertain at restart | Provider explains limits, reconciliation and notices; uncertainty never silently reappears as a fresh allowance |
| S41 | Several vendors sell independent edge/cloud plans on same device | Entitlements and billing merchants stay independent, including authorized reseller cases |
| S42 | Cloud inference described as shared cognition | Shared infrastructure does not falsely imply cross-customer data, conversation or credit sharing |
| S43 | Active-use hours, talk minutes and credits all shown | Each unit and entitlement balance is separately identified and correctly applied |
| S44 | Model version or service tier changes during an active plan | Customer is told of material compatibility, capability, price and entitlement changes |
| S45 | Approved learned routine repeats without fresh inference | Work may be reused locally; no new remote inference event is asserted if none occurred |
| S46 | Repeat task already satisfies desired state | The operator checks actual state and does not invent unnecessary chargeable inference work |
| S47 | Reused task still falls under runtime-hours subscription | Provider may charge the contracted runtime/period without misrepresenting it as a new inference call |
| S48 | Customer chooses alert-only automated postpaid service | Threshold alerts are offered as agreed and billing continues without a hard ORSi stop |
| S49 | Customer explicitly chooses uncapped operation | No ORSi spending ceiling is imposed; accepted provider rates, lawful restrictions and reconciliation still apply |
| S50 | Customer chooses a hard spending cap | Additional chargeable work follows the accepted cap behavior, rather than silently overbilling |
| S51 | Alerts delayed or unavailable during offline use | Provider discloses best-effort delivery and reconciliation/notification behavior |
| S52 | Routine changes or fails verification and requires inference | Actual inference events follow the provider policy; recorded reuse is not asserted when fresh inference occurred |
| S53 | Unlimited workflow access offered under a valid plan | Authorized known tasks continue without a mandatory ORSi invocation cap or fresh inference per repetition |
| S54 | Known routine repeats without a supplier model call | The inference provider is not billed or credited with an event it did not serve |
| S55 | Novel task invokes an independent inference provider | Actual inference is accounted under supplier-defined credits, validity and commercial terms |
| S56 | Operator sells a subscription with routine reuse | Operator service subscription and genuine inference charges remain distinct and accurately disclosed |
| S57 | User reaches expiry, hardware capacity or a published fair-use condition | Unlimited workflow offer does not conceal or override valid contractual, safety and capacity restrictions |
| S58 | Three independent parties participate in a plan | User access, supplier inference charges and AI application-provider service charges can be independently explained |
| S59 | Provider offers unlimited covered workflows for one registered device | The included tasks may repeat within validity without a provider-imposed task-count limit; other devices are not silently covered |
| S60 | Same hardware holds two independent providers' plans | One provider's single-device 'unlimited' entitlement does not overwrite the other's credits or validity |
| S61 | Customer tries covered routines after the plan expires | Published renewal, expiry or grace rules apply; unlimited does not imply permanent validity |
| S62 | Single-device plan invokes separately priced cloud inference | The 'unlimited' covered workflow claim does not silently convert external inference into free usage |
| S63 | Lost/replaced hardware or eligible host changes | Actual enrolled-device binding, host compatibility, rebind and transfer policies are disclosed |
| S64 | Provider independently chooses non-unlimited or multi-device plan | ORSi allows these alternatives without requiring a single global tariff or entitlement scope |
| S65 | Optional feature has no current business requirement | Mark DEFERRED; don't invent a mandatory field or a default |
| S66 | Two providers offer different valid plans | One may include unlimited approved routines while another charges metered credits; both may coexist |
| S67 | Real paid offer leaves material price or service scope undisclosed | A draft PROVIDER_DEFINED placeholder cannot establish informed consent |
| S68 | Subscriber switches device or provider | Telecom analogy does not grant automatic credit/model/identity portability |

The scenarios are for stakeholder review before a future release-candidate profile. They do not prescribe code, test harnesses, device firmware, or payment integrations. Reviewers should register disagreements in `../governance/OPEN-QUESTIONS.md` and decisions separately in `../governance/DECISIONS.md`.
