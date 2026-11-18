# Supplier RFQ / RFP Response Review

**Prompt ID:** COMM-005 | **Category:** Commercial & Project Governance | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Evaluate supplier proposals against procurement requirements to identify compliance gaps, delivery risks, commercial exposure, and clarification needs before vendor selection.

**Use case:** Review RFQ, RFP, tender, or supplier-selection responses for software implementation, SaaS, cloud, infrastructure, and other IT projects.

Copy the prompt and replace the placeholders.

```text
ROLE

You are a Senior IT Project Manager and Procurement Evaluation
Specialist experienced in software delivery, supplier selection,
technology contracts, commercial evaluation, and governance.

CONTEXT

Project: [PROJECT NAME]
Procurement type: [RFQ / RFP / TENDER]
Service / product: [DESCRIPTION]
Evaluation stage: [TECHNICAL / COMMERCIAL / FINAL]
Delivery approach: [PREDICTIVE / AGILE / KANBAN / HYBRID]
Contract model: [FIXED PRICE / TIME & MATERIALS / OTHER]

Approved evaluation criteria: [LIST]
Mandatory requirements: [LIST]
Desirable requirements: [LIST]
Approved scoring weights: [IF AVAILABLE]
Evaluation rules / disqualification criteria: [IF AVAILABLE]

PROCUREMENT REQUIREMENTS

[PASTE RFQ / RFP REQUIREMENTS]

SUPPLIER RESPONSE

[PASTE SUPPLIER PROPOSAL]

OPTIONAL ADDITIONAL SUPPLIERS

[PASTE OTHER RESPONSES IF COMPARISON IS REQUIRED]

TASK

Evaluate the supplier response against the stated requirements.

STEP 1 — REQUIREMENTS COMPLIANCE

1. Map each requirement to the corresponding supplier response.
2. Classify compliance as:
   - Compliant
   - Partially Compliant
   - Non-Compliant
   - Not Provided
   - Requires Clarification
3. Distinguish mandatory requirements from desirable criteria.
4. Verify supporting evidence rather than accepting unsupported claims.
5. Identify deviations, incomplete responses, and missing information.

STEP 2 — TECHNICAL AND DELIVERY EVALUATION

6. Assess relevant technical requirements:
   - Architecture and integrations
   - APIs and data migration
   - Performance and scalability
   - Security and compliance
   - Testing and deployment
   - Support and operational readiness
7. Evaluate delivery methodology, milestones,
   mobilization, resources, and dependencies.
8. Distinguish named and committed personnel
   from illustrative resource profiles.
9. Identify third-party and subcontractor dependencies.
10. Assess alignment between the proposed delivery approach
    and commercial commitments.

STEP 3 — COMMERCIAL EVALUATION

11. Review:
    - Implementation and recurring costs
    - Licensing, cloud, and third-party fees
    - Support and maintenance
    - Change rates and resource rates
    - Taxes, travel, and other relevant costs
12. Extract supplier assumptions and exclusions.
13. Identify potential hidden costs and scope gaps.
14. Assess the three most material commercial risks.
15. Flag costs requiring clarification without assuming
    that missing items are necessarily additional charges.

STEP 4 — PROCUREMENT RECOMMENDATION

16. Generate specific clarification questions linked
    to individual requirements and evidence gaps.
17. Identify the highest-priority technical, commercial,
    security, and delivery risks.
18. Apply approved scoring and weights where supplied.
19. If multiple proposals are provided, compare suppliers
    against identical criteria and evidence standards.
20. Recommend one outcome:
    - Accept for next evaluation stage
    - Accept with conditions
    - Request clarification before progressing
    - Reject

Explain the recommendation using documented evidence
and applicable procurement rules.

RULES

- Do not assume missing information is compliant.
- Do not invent supplier capabilities, certifications,
  resource commitments, costs, or performance evidence.
- Do not invent scoring weights or mandatory requirements.
- Apply evaluation criteria consistently across suppliers.
- Distinguish supplier claims from verified evidence.
- Do not recommend rejection solely because a response
  is incomplete unless procurement rules justify it.
- Identify matters requiring technical, commercial,
  security, or procurement validation.

OUTPUT FORMAT

1. EXECUTIVE ASSESSMENT

Overall Compliance | Main Strengths |
Material Gaps | Procurement Risk |
Recommendation

2. COMPLIANCE MATRIX

Requirement ID | Requirement | Mandatory / Desirable |
Supplier Response | Evidence | Compliance Status |
Gap / Clarification

3. TECHNICAL AND SECURITY REVIEW

Area | Requirement | Supplier Evidence |
Assessment | Delivery / Security Risk

4. COMMERCIAL EVALUATION

Commercial Item | Supplier Position |
Assumption / Exclusion | Potential Exposure |
Clarification Required

5. DELIVERY AND RESOURCE REVIEW

Required Role / Capability | Supplier Proposal |
Availability | Evidence | Gap / Risk

6. KEY SUPPLIER RISKS

Risk | Supporting Evidence | Potential Impact |
Mitigation / Clarification | Priority

7. CLARIFICATION QUESTIONS

ID | Requirement | Question |
Evidence Requested | Priority

8. SUPPLIER COMPARISON (IF APPLICABLE)

Criterion | Approved Weight |
Supplier A | Supplier B | Supplier C |
Evaluation Comment

9. RECOMMENDATION

Recommended Outcome | Supporting Rationale |
Conditions | Outstanding Evidence |
Approval Required

MANAGEMENT SUMMARY

- Supplier suitability
- Mandatory compliance gaps
- Main commercial and delivery exposure
- Required clarifications
- Recommended next procurement action

Use concise Markdown tables.
Mark missing information as "Not Provided".
Do not create unsupported supplier rankings.
```

---

## 2. Quality Check

Apply this independent review before finalizing the supplier evaluation.

```text
QUALITY CHECK

Act as an independent Senior Procurement and PMO
Quality Assurance Manager.

Review the supplier evaluation against the original
RFQ / RFP and supplier response.

Verify:

1. Traceability: Every assessment links to a stated
   requirement and supporting evidence.
2. Compliance: Missing or partial responses are not
   incorrectly classified as compliant.
3. Mandatory Requirements: Potential disqualification
   conditions are identified and applied consistently.
4. Technical Assessment: Claims of capability, security,
   scalability, and implementation experience are supported.
5. Commercial Accuracy: Pricing, assumptions, exclusions,
   and recurring costs are represented correctly.
6. Delivery Feasibility: Resources, milestones, methods,
   and dependencies are assessed.
7. Fairness: Evaluation criteria and approved weights
   are applied consistently without supplier bias.
8. Recommendation: The proposed outcome reflects
   evidence, materiality, and procurement rules.
9. Governance: Outstanding clarifications and required
   approvals are explicitly identified.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent scoring weights, evaluation evidence,
supplier commitments, or procurement decisions.
```

---

## 3. Practical IT Use Case

### CRM Implementation — Supplier Proposal Evaluation

**Scenario:** A company is selecting a supplier for a CRM replacement project. The procurement team has received a proposal that includes a fixed implementation price and relevant experience, but several technical, delivery, and commercial requirements are incompletely addressed.

The Project Manager must identify material gaps before recommending progression to the next procurement stage.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM System Replacement |
| Phase | Procurement / Vendor Selection |
| Procurement type | Request for Proposal |
| Delivery model | Hybrid |
| Contract model | Fixed Price |
| Supplier | CRM Implementation Vendor |
| Proposed price | €920,000 |
| Key concern | Migration, resources, and support coverage |
| Management objective | Determine whether the proposal is sufficiently complete to progress |

### Example Input

```text
Project: CRM System Replacement

Procurement type: RFP
Contract model: Fixed Price

MANDATORY / DESIRABLE CLASSIFICATION
Not provided.

REQUESTED REQUIREMENTS

R-01 Fixed implementation price
R-02 Detailed data migration methodology
R-03 Three comparable CRM project references
R-04 Named Project Manager and Solution Architect
R-05 Detailed project delivery plan
R-06 EU data residency
R-07 ISO 27001 certification
R-08 Twelve months post-go-live support
R-09 Complete technical compliance matrix

SUPPLIER RESPONSE

R-01 Fixed implementation price: €920,000
R-02 Migration approach: Two-page summary
R-03 Two CRM project references provided
R-04 Project Manager CV provided;
     Solution Architect not named
R-05 High-level eight-month timeline
R-06 EU hosting confirmed
R-07 ISO 27001 certificate provided
R-08 Six months support proposed
R-09 Technical compliance matrix 80% complete

Approved scoring weights:
Not provided.

Supplier assumptions and exclusions:
Not provided.
```

### Example Output — Supplier Evaluation

#### 1. Executive Assessment

The supplier has submitted a fixed implementation price of €920,000 and evidence of relevant CRM experience. However, the proposal contains material gaps in migration planning, resource commitments, delivery planning, and post-go-live support.

The supplier also provides fewer project references than requested and an incomplete technical compliance matrix.

**Recommendation: Request clarification before progressing.**

Mandatory compliance and formal eligibility must be confirmed against the approved procurement rules.

#### 2. Compliance Matrix

| ID | Requirement | Supplier Response | Status | Gap |
|---|---|---|---|---|
| R-01 | Fixed price | €920,000 | Compliant | Detailed scope and cost coverage not verified |
| R-02 | Detailed migration methodology | Two-page summary | Partially Compliant | Migration and reconciliation detail missing |
| R-03 | Three project references | Two provided | Partially Compliant | One reference missing |
| R-04 | Named PM and Architect | PM CV only | Partially Compliant | Solution Architect not named |
| R-05 | Detailed project plan | Eight-month summary | Partially Compliant | Milestones and dependencies missing |
| R-06 | EU data residency | EU hosting confirmed | Requires Clarification | Contractual and technical evidence needed |
| R-07 | ISO 27001 certification | Certificate provided | Requires Clarification | Validity and applicable scope require verification |
| R-08 | Twelve months support | Six months offered | Non-Compliant | Support term below requirement |
| R-09 | Full compliance matrix | 80% complete | Partially Compliant | Remaining requirements unanswered |

Classification reflects only the information supplied, not a completed procurement verification.

#### 3. Technical and Security Review

| Area | Supplier Evidence | Assessment | Risk |
|---|---|---|---|
| Architecture | Not provided | Requires clarification | Design feasibility unknown |
| Integration | Not detailed | Incomplete | Scope and dependency uncertainty |
| Data migration | Two-page summary | Insufficient detail | Migration quality and cutover risk |
| Security certification | Certificate supplied | Verification required | Certification scope uncertain |
| Data residency | EU hosting stated | Evidence required | Contractual protection unclear |
| Testing | Not provided | Requires clarification | Acceptance planning uncertainty |

#### 4. Commercial Evaluation

| Item | Supplier Position | Potential Exposure | Clarification |
|---|---|---|---|
| Implementation | €920,000 fixed price | Scope assumptions may affect final cost | Confirm inclusions and exclusions |
| Data migration | Summary only | Additional migration work may require change | Define migration boundaries |
| Support | Six months | Additional support may have a cost | Price the requested 12 months |
| Licensing | Not provided | Potential unpriced fees | Confirm license responsibilities |
| Third-party services | Not provided | Possible external cost exposure | Identify third-party charges |
| Change requests | Not provided | Unclear variation pricing | Provide change rates and process |

The three most material commercial concerns are migration scope, support duration, and unspecified cost exclusions.

#### 5. Delivery and Resource Review

| Requirement | Supplier Proposal | Gap / Risk |
|---|---|---|
| Project Manager | CV supplied | Allocation and availability not confirmed |
| Solution Architect | Not named | Critical design resource unconfirmed |
| Delivery plan | Eight-month overview | Detailed milestones missing |
| Data migration specialist | Not specified | Delivery capacity unknown |
| Testing resources | Not specified | QA responsibility unclear |
| Supplier dependencies | Not specified | External dependency exposure unknown |

#### 6. Key Supplier Risks

| Risk | Supporting Evidence | Potential Impact | Priority |
|---|---|---|---|
| Migration methodology incomplete | Two-page summary | Quality or cutover problems | High |
| Solution Architect unconfirmed | No named resource | Design and mobilization delays | High |
| Insufficient support proposal | Six instead of 12 months | Support coverage gap | High |
| Delivery plan incomplete | High-level timeline only | Unrealistic or unclear milestones | High |
| Technical responses missing | 80% matrix completion | Unknown compliance exposure | High |

Priorities are provisional and require validation against the procurement risk criteria.

#### 7. Clarification Questions

| ID | Requirement | Clarification Question | Priority |
|---|---|---|---|
| Q-01 | Migration | Provide detailed extraction, cleansing, reconciliation, cutover, and rollback methodology | High |
| Q-02 | Solution Architect | Confirm the named architect, experience, availability, and project allocation | High |
| Q-03 | Support | Confirm pricing and scope for the requested 12-month support period | High |
| Q-04 | Project plan | Provide detailed milestones, deliverables, dependencies, and resource allocation | High |
| Q-05 | Security | Provide certificate validity, scope, and relevant security evidence | High |
| Q-06 | Compliance | Complete all outstanding technical compliance matrix items | High |
| Q-07 | Commercial | Identify all assumptions, exclusions, and potential additional costs | High |
| Q-08 | References | Provide the third requested comparable CRM implementation reference | Medium |

#### 8. Supplier Comparison

Not applicable. Only one supplier response was provided.

No weighted score or supplier ranking can be established without the approved evaluation criteria and scoring methodology.

#### 9. Procurement Recommendation

**Recommended outcome: Request clarification before progressing.**

The supplier demonstrates some relevant capabilities, but the proposal is not sufficiently complete to support a final supplier-selection recommendation.

Progression should depend on:

- Resolution of material migration and delivery gaps.
- Confirmation of the named Solution Architect and delivery capacity.
- A compliant or formally accepted support proposal.
- Complete technical and security evidence.
- Clarification of commercial assumptions and exclusions.
- Confirmation of applicable mandatory procurement criteria.

### Management Decisions

1. **Technical suitability:** Require evidence of migration capability, solution architecture, and testing approach.
2. **Delivery confidence:** Confirm resource commitments and obtain a realistic implementation schedule.
3. **Commercial completeness:** Clarify the fixed-price scope, exclusions, and twelve-month support requirement.
4. **Procurement governance:** Determine whether the supplier may progress after clarification under the approved evaluation rules.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The evaluation identifies key compliance, technical, resource, and commercial gaps. However, mandatory requirement classifications, scoring methodology, certification validity, and detailed pricing coverage remain unverified.

**Required corrections:**
- Obtain approved mandatory-versus-desirable requirement classifications.
- Verify supplier certification and technical evidence.
- Complete missing procurement responses.
- Confirm commercial assumptions and exclusions.
- Validate the recommendation against procurement rules.

**Approval blockers:** Incomplete supplier evidence, unresolved material compliance gaps, and unavailable approved evaluation criteria.

**Governance:** Supports PMI-aligned procurement management, supplier selection, quality assurance, risk management, financial oversight, and project governance.

AI-assisted supplier evaluations support evidence-based comparison but do not replace authorized procurement decisions. All supplier assessments, commercial conclusions, and recommendations require appropriate Procurement, Technical, Security, and Commercial review. Protect confidential pricing, rate cards, architecture, security evidence, and supplier proposals.
