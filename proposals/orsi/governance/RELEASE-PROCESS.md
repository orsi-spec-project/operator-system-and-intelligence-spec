# ORSi Spec — proposed review, governance and dated releases

**Status: proposal only — not adopted governance, a standards body, conformance program or an approved public release.** The ORSi-01 core text is editorially review-ready within prep; stakeholder acceptance and naming/IP clearance remain pending.

ORSi Spec is independent of MCP. The Model Context Protocol uses dated revisions such as `2026-07-28`, statuses including Draft/Current/Final, and a proposal/release-review process. ORSi Spec proposes a lightweight equivalent for commercial entitlement definitions, not the MCP transport, wire protocol, or server interfaces.

## Revision naming

- Working revision: `YYYY-MM-DD-DRAFT` (current package: `2026-11-18-DRAFT`).
- Editorial review-ready draft: the current `YYYY-MM-DD-DRAFT` has coherent proposed terms but still needs owner/stakeholder acceptance. This is **not** an RC.
- Candidate revision: `YYYY-MM-DD-RC1`, `RC2`, etc., only after a documented stakeholder/owner acceptance and review freeze.
- Stable revision: `YYYY-MM-DD`, only when accepted and formally released.
- Historical stable revisions: retained unchanged as `Final` when superseded, with clear compatibility notes.

A date is a revision identity, not a promise of publication on that date. The current package is a preparation draft and MUST NOT be represented as a stable release.

## Editorial acceptance gate

Before a draft may advance to an RC, reviewers SHOULD check the common terms for minimal scope, distinct credits/talk time/validity, conditional applicability, independent providers, clear billing responsibility, accurate 'unlimited' claims, USB/device trust limitations, offline accounting honesty and protection of customer privacy.

**Sector-neutral participation is a core editorial requirement:** ORSi is open to inference/model providers, AI developers and other voluntary adopters. Telecom and flash-memory/USB sectors are illustrative references only; **neither owns, governs, vetoes or has compulsory participation or exclusive commercial rights by industry role**. No manufacturer, telecom operator or sector-specific representative is required to approve a draft. Relevant technical reviewers are selected for the claims being made. Industry opportunities MUST NOT be presented as compulsory business models, proven adoption, guaranteed revenue or third-party endorsement.

No formal conformance certificate can be inferred from written scenarios. Contributor IP, trademark clearance, named publishing steward and explicit owner acceptance are release blockers, not silently deferred customer features.

## Release gates

1. **Explore:** publish motivation and open questions; avoid private product implementation details.
2. **Draft:** define terms, minimum fields, payment modes, coexistence and precise examples.
3. **Review:** obtain relevant inference/model, AI developer and customer viewpoints, plus security, device or other technical expertise **where the proposed claims require it**. No telecom or USB/OEM industry membership or sponsor is compulsory. Resolve material security and consumer-rights objections.
4. **Candidate:** freeze normative semantics; add human-readable conformance scenarios and backwards-compatibility notes.
5. **Published:** after separate approval, publish an explicit version, change log, approved governance and license/rights notices in `operator-system-and-intelligence-spec`. Any conformance claim requires its own defined acceptance and evidence process.
6. **Final/superseded:** preserve older accepted revisions, migration and deprecation guidance.

There is no automatic release date or claim of community consensus. A release manager/steward should be identified before RC.

## Change proposals (ORSi Enhancement Proposals, or OEPs — draft process)

Each proposal should state: challenge, affected parties, changed terms/fields, incentives and abuse risks, privacy, backward compatibility, examples, disagreements, decision, and review evidence. Keep unresolved changes out of stable releases.

## Governance rules under discussion

- Vendor-neutral participation and transparent decision logs.
- No single inference provider may redefine another provider's entitlement or require a central settlement service.
- Distinguish normative commercial terms from implementation suggestions.
- Owner-selected scope: Apache-2.0 formal specifications and future code; CC BY 4.0 supporting docs, per [LICENSING.md](../../../LICENSING.md). Contributor IP/patents, brand policy and formal publication authority still require review.
- Record security assumptions and unresolved limitations; do not claim offline accounting is inherently tamper-proof.
- Corrections affecting customer rights or existing bills require explicit compatibility analysis.

## Business-driven progressive releases

The first profile deliberately leaves detailed commercial designs open. Only the minimum shared meaning is a common candidate; providers independently choose tariff structure, validity, credits, included routines, optional unlimited offers, recharge and spending controls.

A proposed extension must identify a real customer or provider need, conditional vs common applicability, affected rights, acceptance scenarios and compatibility. Neither an undocumented paid contract nor an unverified hardware guarantee becomes valid merely because a specification placeholder is DEFERRED.

See the [Progressive Policy](PROGRESSIVE-SPECIFICATION.md), [Deferred Decision Register](DEFERRED-DECISIONS.md), and separately maintained non-normative telecom case studies.

## Repository review and publication authority

A draft may be prepared on a parking branch, then copied for **review-draft integration** into the specification repository with explicit owner authorization. Parking alone does **not** grant approval. **Integration of a draft is not standards ratification, an RC, an adoption claim, certification or a stable release**. A future stable release requires separately documented acceptance of the scoped requirements, applicable stakeholder evidence, approved rights and named stewardship.

The source and editorial history remain preserved in the preparation repository. Case studies and optional industry economics remain outside the core standard and may be discussed separately on demand.

## Background references

- [MCP Versioning](https://github.com/modelcontextprotocol/modelcontextprotocol/blob/main/docs/docs/2026-07-28/learn/versioning.mdx)
- [MCP: A More Predictable Release Cycle (11 November 2026)](https://blog.modelcontextprotocol.io/posts/mcp-release-cycle/)
