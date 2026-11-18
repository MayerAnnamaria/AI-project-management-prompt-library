# Contract Clause Analysis

**Prompt ID:** COMM-001 | **Category:** Commercial & Project Governance | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Translate contractual requirements into practical project-management obligations, risks, dependencies, and controls without replacing professional legal interpretation.

**Use case:** Review IT implementation, SaaS, cloud, or vendor contract clauses when delivery responsibilities, acceptance criteria, deadlines, payments, or change-control obligations affect project execution.

Copy the prompt and replace the placeholders with your contract information.

```text
ROLE

You are a Senior IT Project Manager and Commercial Management
Specialist experienced in software implementation, SaaS,
vendor contracts, procurement, and project governance.

CONTEXT

Project: [PROJECT NAME]
Project phase: [PHASE]
Contract type: [SOFTWARE / SAAS / CLOUD / OUTSOURCING / OTHER]
Customer: [ROLE]
Supplier: [ROLE]
Delivery approach: [PREDICTIVE / AGILE / KANBAN / HYBRID]
Commercial context: [DETAILS]
Related clauses: [IF AVAILABLE]
Contract version: [VERSION / DATE]

CONTRACT CLAUSE

[PASTE EXACT CLAUSE]

OPTIONAL COMPARISON

Previous clause version: [PASTE / NOT AVAILABLE]

TASK

Analyze the clause from a project-management and commercial
governance perspective.

STEP 1 — INTERPRET REQUIREMENTS

1. Explain the clause in 2–4 plain-English sentences.
2. Identify explicit Customer and Supplier obligations.
3. Extract deadlines, triggers, conditions, notice periods,
   and acceptance requirements.
4. Identify the consequence of non-compliance only when
   expressly supported by the supplied contract text.
5. Flag ambiguous language, missing definitions,
   and related clauses requiring review.

STEP 2 — ASSESS PROJECT IMPLICATIONS

6. Identify potential impacts on:
   - Schedule and milestones
   - Scope and deliverables
   - Acceptance and quality
   - Payments and commercial exposure
   - Dependencies and responsibilities
   - Change control and governance
   - Security, compliance, or operations where relevant

7. Distinguish confirmed contractual requirements from
   potential risks and assumptions.
8. Assess commercial and delivery risks separately
   for the Customer and Supplier.
9. Identify critical inter-party dependencies and
   potential areas of disagreement.
10. Challenge the analysis from the counterparty's
    perspective to expose unsupported interpretations.

STEP 3 — DEFINE PROJECT CONTROLS

11. Translate material obligations into operational controls:
    - Obligations register
    - Deliverable acceptance tracker
    - Contractual notice tracker
    - Dependency and decision logs
    - Change-control register
    - Vendor performance monitoring

12. Recommend responsible roles, evidence, review points,
    and escalation triggers.
13. Generate clarification questions for Legal, Procurement,
    Commercial Management, or the relevant stakeholders.
14. If two clause versions are supplied, identify changes
    to obligations, deadlines, risk allocation, and delivery.
15. Highlight matters requiring legal interpretation
    or formal contractual approval.

RULES

- Analyze only the text and context actually provided.
- Do not invent contractual rights, remedies, obligations,
  waivers, breaches, termination rights, or liabilities.
- Distinguish clause-derived facts from possible implications.
- Do not assume a contractual term has a particular legal
  effect without considering applicable law and other terms.
- Refer legal conclusions to qualified Legal counsel.
- Recommend only controls that serve a practical purpose.

OUTPUT FORMAT

1. PLAIN-ENGLISH SUMMARY

Clause Purpose | Key Requirement | Business Implication

2. CONTRACTUAL OBLIGATIONS

Party | Obligation | Trigger | Deadline |
Required Evidence | Clause Reference

3. DEADLINES AND CONDITIONS

Trigger | Required Action | Responsible Party |
Deadline | Express Contractual Consequence

4. PROJECT DELIVERY IMPLICATIONS

Area | Contract Requirement | Potential Impact |
Project Control | Proposed Owner

5. COMMERCIAL AND DELIVERY RISKS

Affected Party | Risk Scenario | Potential Impact |
Preventive Control | Evidence Required

6. AMBIGUITIES AND CLARIFICATIONS

Clause Wording | Possible Interpretations |
Project Concern | Clarification Required

7. CONTRACT OBLIGATIONS REGISTER

ID | Clause | Obligation | Party | Trigger |
Deadline | Proposed Owner | Evidence | Status

8. CONTRACT VERSION COMPARISON (IF APPLICABLE)

Change | Version A | Version B |
Operational / Commercial Implication |
Legal Review Required?

9. MANAGEMENT SUMMARY

- Critical contractual obligations
- Main delivery and commercial exposures
- Recommended project controls
- Unresolved interpretation questions
- Required stakeholder or legal review

Use concise Markdown tables.
Mark unsupported conclusions as "Requires legal review".
Do not present operational recommendations as legal obligations.
```

---

## 2. Quality Check

Apply this independent review before using the analysis for project decisions or contractual communication.

```text
QUALITY CHECK

Act as a Senior PMO Quality Assurance Manager with experience
in IT procurement and commercial governance.

Review the clause analysis against the original wording.

Verify:

1. Fidelity: Summaries accurately reflect the actual clause.
2. Obligations: Customer and Supplier duties are separated
   and supported by specific wording.
3. Timing: Deadlines, triggers, and conditions are accurate.
4. Consequences: No unsupported contractual remedies,
   liability, or legal conclusions have been invented.
5. Interpretation: Ambiguities, related clauses, and
   alternative counterparty interpretations are identified.
6. Delivery: Project implications and dependencies are logical.
7. Commercial Risks: Risks are proportionate and distinguish
   actual contractual exposure from hypothetical scenarios.
8. Controls: Recommendations are actionable, proportionate,
   and linked to obligations.
9. Governance: Legal, Procurement, or Commercial review
   requirements are appropriately identified.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Legal / Commercial Review Required: [OPEN QUESTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not assume missing contractual provisions or
make definitive legal determinations.
```

---

## 3. Practical IT Use Case

### Software Implementation — Deliverable Acceptance Clause

**Scenario:** A company is implementing a new CRM system with an external software vendor. The contract requires the customer to review submitted deliverables within five business days. If no response is provided, the deliverable is deemed accepted.

The Project Manager must establish an acceptance process to prevent missed review deadlines and unclear responsibilities.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM System Implementation |
| Phase | Configuration / Deliverable Acceptance |
| Contract type | Software Implementation Agreement |
| Customer | Internal Business / IT Team |
| Supplier | CRM Implementation Vendor |
| Key requirement | Five-business-day acceptance period |
| Main exposure | Deliverables deemed accepted without an explicit customer response |
| Management objective | Define acceptance ownership, tracking, and escalation |

### Example Input

```text
Project: CRM System Implementation
Contract type: Software Implementation Agreement

Customer: Internal Business / IT Team
Supplier: CRM Implementation Vendor

Clause:

"The Customer shall review each Deliverable within five
Business Days of receipt and either approve it or provide
written details of any material non-conformance with the
agreed Acceptance Criteria.

If no response is received within that period,
the Deliverable shall be deemed accepted."

Project context:
- Vendor submits configured CRM functionality for review.
- Business Owner and QA Lead participate in acceptance.
- Several deliverables are planned during configuration.
- No centralized acceptance tracker currently exists.

Related contractual definitions:
Not provided.

Task:
Identify obligations, risks, deadlines, and project controls.
```

### Example Output — Contract Clause Analysis

#### 1. Plain-English Summary

The customer must review each received deliverable within five business days and either approve it or provide written details of material non-conformance with the agreed acceptance criteria.

If the customer does not respond within that period, the clause states that the deliverable is deemed accepted. The effect of such acceptance under the wider agreement requires legal review.

#### 2. Contractual Obligations

| Party | Obligation | Trigger | Deadline |
|---|---|---|---|
| Customer | Review each deliverable | Receipt of deliverable | Within 5 business days |
| Customer | Approve or provide written non-conformance details | Deliverable review | Within review period |
| Supplier | No separate express submission duty stated in this excerpt | Not specified | Not specified |

The clause refers to supplier deliverables, but the supplier's full delivery obligations must be established from other contract provisions.

#### 3. Deadlines and Conditions

| Trigger | Required Action | Responsible Party | Consequence |
|---|---|---|---|
| Deliverable received | Start review process | Customer | Review period begins |
| Review period active | Approve or provide written objections | Customer | Response required within 5 business days |
| No response within review period | No further action stated | Customer | Deliverable deemed accepted under clause |

**Clarification required:** The contract's definition of *Business Day*, applicable holidays, receipt method, and any other notice requirements.

#### 4. Project Delivery Implications

| Area | Potential Impact | Recommended Control |
|---|---|---|
| Schedule | Short acceptance windows require coordinated review | Acceptance calendar |
| Quality | Review may be incomplete before deadline | Acceptance checklist |
| Governance | Approval responsibility may be unclear | Named acceptance owner |
| Commercial | Deemed acceptance may affect later contractual processes | Legal review of related provisions |
| Documentation | Unrecorded responses may create disputes | Central evidence repository |

#### 5. Commercial and Delivery Risks

| Affected Party | Risk Scenario | Potential Impact | Preventive Control |
|---|---|---|---|
| Customer | Acceptance deadline missed | Deemed acceptance | Automated deadline alerts |
| Customer | Material defects not documented in writing | Unclear acceptance position | Standard non-conformance template |
| Supplier | Approval or rejection communication is unclear | Potential dispute | Defined submission and response channels |
| Both | Acceptance criteria interpreted differently | Rework or disagreement | Confirmed acceptance criteria baseline |

These are potential operational and commercial risks, not conclusions that either party has breached the contract.

#### 6. Ambiguities and Clarifications

| Wording | Concern | Clarification Required |
|---|---|---|
| "Business Days" | Calendar calculation | Which holidays and jurisdictions apply? |
| "Receipt" | Unclear review start | What constitutes valid delivery? |
| "Material non-conformance" | Different interpretations | How is materiality assessed? |
| "Agreed Acceptance Criteria" | Missing reference | Which approved version applies? |
| "Deemed accepted" | Wider legal implications | How does acceptance interact with defects, warranties, and payments? |

#### 7. Contract Obligations Register

| ID | Obligation | Party | Trigger | Proposed Owner | Evidence |
|---|---|---|---|---|---|
| C-01 | Review deliverables within 5 business days | Customer | Receipt | Business Owner | Review record |
| C-02 | Provide written approval or non-conformance details | Customer | Review outcome | Authorized Approver | Written response |
| C-03 | Track acceptance deadlines | Internal project control | Receipt | Project Manager | Acceptance tracker |
| C-04 | Escalate approaching deadlines | Internal project control | Review outstanding | Project Manager | Escalation record |

C-03 and C-04 are **recommended project controls**, not additional contractual duties created by the clause.

#### 8. Contract Version Comparison

Not applicable. Only one clause version was provided.

### Management Decisions

1. **Acceptance ownership:** Confirm who reviews deliverables and who is authorized to approve them.
2. **Deadline control:** Introduce a centralized acceptance tracker with early alerts before each five-business-day deadline.
3. **Quality:** Agree on review evidence and written non-conformance documentation.
4. **Commercial governance:** Ask Legal or Procurement to confirm the operation of deemed acceptance under the full agreement.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The analysis identifies the customer review obligation and deemed-acceptance condition. It distinguishes express contractual requirements from proposed project controls. However, critical definitions and related provisions are unavailable.

**Required corrections:**
- Verify the definition of *Business Day* and *receipt*.
- Review the complete acceptance and notice provisions.
- Confirm approval authority and acceptance criteria.
- Validate any commercial implications with Legal or Procurement.
- Implement the acceptance tracker after process approval.

**Legal / Commercial Review Required:** Deemed-acceptance implications, defect-remedy provisions, and relationships with payment or warranty clauses.

**Approval blockers:** Incomplete contractual context and unconfirmed acceptance authority.

**Governance:** This framework supports PMI-aligned procurement management, vendor governance, stakeholder responsibilities, risk management, and contract administration.

AI-assisted clause analysis is for project-management awareness and operational planning. It is not legal advice. Material contractual conclusions, formal notices, and commercial decisions require review by qualified professionals. Protect confidential contract terms, pricing, security provisions, and personal data.
