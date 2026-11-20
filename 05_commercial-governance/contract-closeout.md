# Contract Close-Out

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** COMM-006 | **Category:** Commercial & Project Governance

---


## 1. Ready-to-Use Prompt

**Purpose:** Verify that contractual, financial, technical, and operational obligations have been completed or formally transferred before supplier contract closure.

**Use case:** Prepare contract close-out documentation during software deployment, operational handover, hypercare exit, or final supplier reconciliation when formal acceptance and commercial closure are required.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager and Commercial Manager
experienced in supplier governance, financial reconciliation,
contract administration, operational transition, and project closure.

CONTEXT

Project: [PROJECT NAME]
Contract / type: [NAME / SOFTWARE / SAAS / CLOUD / OTHER]
Customer: [PARTY]
Supplier: [PARTY]
Delivery approach: [PREDICTIVE / AGILE / KANBAN / HYBRID]
Current phase: [DEPLOYMENT / HANDOVER / HYPERCARE / CLOSE]

COMMERCIAL DATA

Original contract value: [AMOUNT]
Approved changes: [LIST / AMOUNT]
Adjusted contract value: [AMOUNT]
Supplier final account: [AMOUNT]
Agreed final position: [AMOUNT / NOT YET AGREED]
Invoices and payments: [DETAILS]
Credits / claims / retentions: [DETAILS]
Contingency: [APPROVED / USED / REMAINING]
Outstanding commitments: [DETAILS]

DELIVERY AND HANDOVER DATA

Contracted deliverables: [LIST / STATUS]
Acceptance records: [DETAILS]
Outstanding defects: [DETAILS]
Data migration / integrations: [STATUS]
Technical documentation: [STATUS]
Security / compliance: [STATUS]
Operational handover: [STATUS]
Support / warranty arrangements: [DETAILS]
Hypercare exit: [STATUS]
Open risks / issues: [LIST]
Vendor performance evidence: [IF AVAILABLE]
Required closure approvals: [ROLES / CONTRACT REFERENCES]

TASK

Prepare a Contract Close-Out Package comprising a final
commercial narrative and a structured closure checklist.

STEP 1 — COMMERCIAL RECONCILIATION

1. Reconcile:
   Original Contract + Approved Changes = Adjusted Value.
2. Compare the adjusted value, supplier final submission,
   agreed final account, and recorded payments.
3. Calculate and explain supported variances.
4. Review contingency use, pending credits, claims,
   invoices, change requests, and outstanding commitments.
5. Flag duplicate charges, unsupported costs,
   and reconciliation gaps.
6. Do not treat a supplier submission as an agreed settlement.

STEP 2 — TECHNICAL AND OPERATIONAL CLOSURE

7. Verify contracted deliverables, acceptance evidence,
   deployment, integrations, migration, and quality criteria.
8. Identify unresolved defects, severity, disposition,
   accountable owner, deadline, and acceptance evidence.
9. Assess documentation currency, approval, completeness,
   accessibility, and operational usability.
10. Review security approvals, compliance evidence,
    temporary access, and outstanding exceptions.
11. Confirm operational ownership, incident procedures,
    monitoring, backup/recovery, support contacts,
    service agreements, and knowledge transfer.
12. Validate hypercare exit against agreed criteria,
    not merely the planned end date.

STEP 3 — GOVERNANCE AND FINAL DECISION

13. Review business, technical, operational, and security
    acceptance evidence.
14. Identify risks, issues, technical debt, and obligations
    requiring formal transfer and recipient acknowledgment.
15. Confirm Finance, Procurement, PMO, and relevant
    contractual closure requirements.
16. Summarize supplier performance using available evidence.
17. Identify final lessons learned and archive requirements.
18. Recommend one closure status:
    - Ready to Close
    - Ready to Close with Conditions
    - Not Ready to Close
19. List approval blockers, conditional obligations,
    accountable owners, and follow-up deadlines.

Adapt closure activities to the contract and delivery model.
For Agile products, distinguish contract closure from
ongoing product development and backlog ownership.

Do not invent contract values, settlement agreements,
acceptance decisions, approvals, or transferred ownership.

Do not automatically recommend closure because production
deployment or hypercare has ended.

OUTPUT FORMAT

1. FINAL COMMERCIAL NARRATIVE

Summarize:
- Original contract position
- Approved changes and adjusted value
- Supplier final submission
- Agreed commercial position
- Variances and contingency
- Outstanding financial obligations
- Commercial closure recommendation

2. FINANCIAL RECONCILIATION

Measure | Amount | Evidence | Status

3. OUTSTANDING COMMERCIAL ITEMS

Item | Amount | Owner | Required Action |
Deadline | Status

4. CONTRACT CLOSE-OUT CHECKLIST

Category | Closure Requirement | Evidence |
Status | Owner | Required Action

Categories:
- Commercial
- Technical and Quality
- Documentation
- Security and Compliance
- Operational Handover
- Stakeholder Acceptance
- Internal Governance

5. DEFECT AND OBLIGATION TRANSFER

Item | Severity / Impact | Disposition |
Receiving Owner | Target Date |
Acceptance Evidence

6. DOCUMENTATION AND HANDOVER

Document / Service | Required | Delivered |
Approved | Receiving Owner | Evidence

7. VENDOR PERFORMANCE REVIEW

Area | Assessment | Evidence |
Future Recommendation

8. CLOSURE READINESS DECISION

Recommended Status | Supporting Rationale |
Outstanding Conditions | Approval Authority |
Closure Blockers

9. FINAL MANAGEMENT ACTIONS

Action | Proposed Owner | Deadline |
Required Evidence | Decision / Approval

Use concise Markdown tables.
Mark unknown information as "Not provided".
Separate confirmed completion from pending approval.
```

---

## 2. Quality Check

Apply this independent review before recommending formal contract closure.

```text
QUALITY CHECK

Act as an independent Senior PMO and Commercial Assurance Reviewer.

Review the Contract Close-Out Package against its source evidence.

Verify:

1. Financial Accuracy: Original value, approved changes,
   adjusted value, final account, invoices, and variances reconcile.
2. Commercial Completeness: Claims, credits, commitments,
   change requests, and outstanding payments are addressed.
3. Deliverable Acceptance: Contracted outputs have evidence
   of completion and appropriate approval.
4. Defect Management: Remaining defects have authorized
   disposition, ownership, deadlines, and traceability.
5. Documentation: Required records are current,
   approved, accessible, and usable by Operations.
6. Security: Access, compliance, vulnerabilities,
   and exceptions have appropriate closure evidence.
7. Handover: Support ownership, incident management,
   monitoring, recovery, and knowledge transfer are established.
8. Governance: Formal acceptance, conditional obligations,
   and approval authority are correctly represented.
9. Closure Decision: Recommendation reflects evidence
   and does not conceal unresolved obligations.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [UNRESOLVED CRITICAL ITEMS]
Recommended closure status:
[READY / CONDITIONAL / NOT READY]

Do not infer financial agreement or formal acceptance
from delivery status alone.
Do not approve closure on behalf of stakeholders.
```

---

## 3. Practical IT Use Case

### CRM Implementation — Supplier Contract Close-Out

**Scenario:** A company has completed a CRM replacement project. Production deployment and hypercare are finished, but final contract reconciliation and formal transfer of two Medium-severity defects must be confirmed before supplier closure.

The Project Manager must demonstrate that commercial, technical, and operational responsibilities have been resolved or appropriately transferred.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM System Replacement |
| Phase | Hypercare Exit / Contract Close |
| Contract type | Software Implementation Agreement |
| Supplier | CRM Implementation Partner |
| Original contract | €1,800,000 |
| Approved changes | €160,000 |
| Adjusted contract | €1,960,000 |
| Agreed final position | €1,985,000 |
| Outstanding technical items | Two Medium defects |
| Management decision | Determine whether conditional closure is justified |

### Example Input

```text
Project: CRM System Replacement

Contract: Software Implementation Agreement
Phase: Hypercare Exit / Contract Close

Original contract value: €1,800,000

Approved changes:
CR-04 — Additional integration: €80,000
CR-09 — Migration scope extension: €55,000
CR-12 — Additional hypercare: €25,000

Supplier final submission: €2,040,000
Agreed final commercial position: €1,985,000

Invoices / payments:
Not provided.

Contingency:
Not provided.

Commercial status:
Final account reported as agreed.
Payment and outstanding commitment status not confirmed.

Delivery:
- CRM is live in production.
- Hypercare completed.
- Business acceptance reported as complete.
- Two Medium defects remain open.
- Defects are planned for BAU resolution.
- Final security approval received.
- Technical documentation complete.
- Operations runbook approved.
- 12-month vendor support active.

Outstanding verification:
- Formal defect acceptance and receiving owner
- Final invoice and payment reconciliation
- Contract closure authority
```

### Example Output — Contract Close-Out Package

#### 1. Final Commercial Narrative

The original CRM implementation contract was valued at **€1,800,000**. Three approved changes totaling **€160,000** increased the adjusted contract value to **€1,960,000**.

The supplier submitted a final account of **€2,040,000**, while the reported agreed final position is **€1,985,000**. This is €55,000 below the supplier's final submission and €25,000 above the adjusted contract value.

Although the final position is reported as agreed, the available information does not establish which additional items explain the €25,000 difference, whether all invoices have been paid, or whether outstanding commitments remain.

**Commercial conclusion:** The reported final account requires reconciliation evidence and Finance confirmation before formal closure.

#### 2. Financial Reconciliation

| Measure | Amount | Status |
|---|---:|---|
| Original contract | €1,800,000 | Provided |
| Approved changes | €160,000 | Provided |
| Adjusted contract | €1,960,000 | Reconciled |
| Supplier final submission | €2,040,000 | Provided |
| Reported agreed final position | €1,985,000 | Evidence required |
| Variance against adjusted contract | +€25,000 | Explanation required |
| Difference from supplier submission | −€55,000 | Reconciliation required |
| Payments and open liabilities | Not provided | Unverified |

The figures reconcile arithmetically but do not, by themselves, establish a complete commercial settlement.

#### 3. Outstanding Commercial Items

| Item | Amount | Proposed Owner | Required Action | Status |
|---|---|---|---|---|
| Final account variance | €25,000 | Commercial Manager | Validate approved basis | Open |
| Supplier submission difference | €55,000 | Commercial Manager | Obtain reconciliation record | Open |
| Final invoices / payments | Unknown | Finance | Confirm settlement | Unverified |
| Purchase order commitments | Unknown | Procurement | Confirm closure | Unverified |
| Contingency use | Unknown | Project Manager / Finance | Reconcile allocation | Unverified |

#### 4. Contract Close-Out Checklist

| Category | Closure Requirement | Evidence / Current Position | Status |
|---|---|---|---|
| Commercial | Final values and payments reconciled | Final amounts provided; settlement evidence missing | Pending |
| Technical | Production deployment completed | CRM reported live | Reported Complete |
| Quality | Remaining defects resolved or accepted | Two Medium defects planned for BAU | Pending |
| Documentation | Technical documents and runbook delivered | Reported complete / approved | Requires verification |
| Security | Final approval received | Approval reported | Reported Complete |
| Operations | Support ownership established | 12-month vendor support active | Partially confirmed |
| Stakeholder Acceptance | Business acceptance completed | Reported complete | Evidence required |
| Governance | Contract closure approved | Authority not provided | Pending |

#### 5. Defect and Obligation Transfer

| Item | Severity | Disposition | Receiving Owner | Evidence |
|---|---|---|---|---|
| Defect D-01 | Medium | Proposed BAU resolution | Not confirmed | Acceptance required |
| Defect D-02 | Medium | Proposed BAU resolution | Not confirmed | Acceptance required |

Defect IDs are illustrative placeholders; the actual defect references were not supplied.

**Required control:** Each remaining defect must have an agreed disposition, accountable receiving owner, target date, and authorized acceptance where required.

#### 6. Documentation and Handover

| Document / Service | Current Position | Required Validation |
|---|---|---|
| Technical documentation | Complete | Confirm current approved version |
| Operations runbook | Approved | Confirm receiving team access |
| Vendor support | Active for 12 months | Confirm scope, escalation, and support start/end dates |
| Incident management | Not provided | Confirm support process |
| Monitoring / backup | Not provided | Confirm operational readiness |
| Knowledge transfer | Not provided | Obtain receiving-team confirmation |
| Temporary project access | Not provided | Confirm access review |

#### 7. Vendor Performance Review

| Area | Assessment | Evidence | Future Recommendation |
|---|---|---|---|
| Deployment | Completed as reported | Production live | Verify acceptance evidence |
| Documentation | Reported complete | Runbook and technical documents | Confirm usability |
| Support | Active | 12-month support arrangement | Monitor early BAU performance |
| Commercial | Pending verification | Final-account discrepancy | Complete reconciliation |
| Quality | Open obligations | Two Medium defects | Track accepted resolution commitments |

No supplier-wide performance rating is justified from the limited information.

#### 8. Closure Readiness Decision

**Recommended status: Not Ready to Close**

Production deployment, hypercare completion, security approval, and active vendor support are positive indicators. However, outstanding financial reconciliation, unverified formal acceptance records, and incomplete defect-transfer evidence prevent a defensible unconditional or conditional closure recommendation.

A **Ready to Close with Conditions** decision may become appropriate if authorized stakeholders confirm that remaining obligations can be contractually closed or transferred while preserving the required rights, controls, and accountability.

#### 9. Final Management Actions

| Action | Proposed Owner | Required Evidence | Timing |
|---|---|---|---|
| Reconcile final account | Commercial Manager | Approved settlement breakdown | Before closure |
| Confirm final payments | Finance | Invoice and payment reconciliation | Before closure |
| Formalize defect transfer | QA / Operations Lead | Accepted defect records | Before closure |
| Validate operational handover | Service Owner | Support and knowledge-transfer sign-off | Before closure |
| Verify acceptance records | Business Owner | Signed acceptance evidence | Before closure |
| Obtain contract closure approval | Authorized Contract Owner | Formal closure decision | After prerequisites |

### Management Decisions

1. **Commercial close-out:** Confirm the €1,985,000 final position and resolve the €25,000 variance against the adjusted contract.
2. **Defect transfer:** Obtain formal acceptance and operational ownership for the two Medium defects.
3. **Service transition:** Verify support readiness, documentation access, and post-hypercare responsibilities.
4. **Contract closure:** Authorize closure only when financial, technical, and governance prerequisites are satisfied or validly addressed through approved conditions.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The commercial figures reconcile arithmetically, and major delivery milestones are reported complete. However, final account evidence, payment status, defect acceptance, operational handover records, and closure authority remain incomplete.

**Required corrections:** Obtain Finance and Commercial confirmation; verify accepted deliverables and defect transfers; confirm support and access controls; document formal approval authority.

**Approval blockers:** Unreconciled commercial variance, incomplete outstanding-obligation evidence, and missing contract closure authorization.

**Recommended closure status:** **Not Ready to Close** until these blockers are resolved or formally addressed by the authorized parties.

**Governance:** Supports PMI-aligned procurement closure, financial control, quality management, operational transition, supplier governance, and project closure.

Contract closure requires authorized human review and must follow the governing agreement. AI cannot settle claims, approve financial accounts, accept deliverables, or terminate contractual obligations. Protect confidential pricing, commercial settlements, supplier performance, customer data, and security information.
