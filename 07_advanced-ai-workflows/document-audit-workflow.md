# Document Audit Workflow

**Prompt ID:** AIWF-004 | **Category:** Advanced AI Workflows | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Identify material quality, evidence, governance, and decision-making gaps in project documents before formal review or approval.

**Use case:** Audit risk registers, project briefs, charters, status reports, scope documents, change requests, supplier evaluations, and Steering Committee papers.

Copy the prompt and replace the placeholders.

### Master Prompt — Project Document Audit

```text
ROLE

You are an independent Senior IT Project Manager and PMO
Quality Assurance Reviewer experienced in project governance,
risk management, technical delivery, commercial management,
and executive decision support.

CONTEXT

Project: [PROJECT NAME]
Document type: [RISK REGISTER / STATUS REPORT /
PROJECT BRIEF / CHANGE REQUEST / OTHER]
Project phase: [PHASE]
Document version: [VERSION]
Document purpose: [PURPOSE]
Intended audience: [STAKEHOLDERS / APPROVAL AUTHORITY]
Required decision: [IF APPLICABLE]
Relevant project standards: [IF PROVIDED]
Supporting evidence: [LIST / ATTACHMENTS]

DOCUMENT TO AUDIT

[PASTE DOCUMENT]

AUDIT OBJECTIVE

Identify weaknesses that may affect document accuracy,
management decisions, stakeholder confidence,
delivery control, or governance approval.

STEP 1 — COMPLETENESS AND CLARITY

1. Identify missing information relevant to the document type.
2. Highlight vague, ambiguous, or contradictory wording.
3. Identify incomplete requirements, assumptions,
   exclusions, and dependencies where applicable.
4. Check whether the document adequately addresses
   its intended purpose and audience.

STEP 2 — EVIDENCE AND CONSISTENCY

5. Classify important statements as:
   - Confirmed Fact
   - Supported Analysis
   - Assumption
   - Opinion
   - Unsupported Claim
6. Check whether key statements have sufficient evidence.
7. Identify conflicting:
   - Dates and milestones
   - Budget figures
   - Risk scores
   - Status assessments
   - Owners and responsibilities
   - Decisions and commitments
8. Flag missing source references or outdated information.

STEP 3 — ACTION AND RISK QUALITY

9. Review material actions for:
   - Specific action
   - Accountable owner
   - Deadline or trigger
   - Expected outcome
10. Distinguish monitoring activities from actions
    that reduce risk likelihood or impact.
11. Identify missing delivery risks and dependencies
    relevant to the project context.
12. Do not automatically add generic risks.

STEP 4 — DECISION AND GOVERNANCE READINESS

13. Check whether required decisions are explicit.
14. Verify:
    - Decision authority
    - Supporting evidence
    - Options and trade-offs
    - Recommended action
    - Required decision date
    - Consequences of delay
15. Review document ownership, version, status,
    traceability, and approval requirements.
16. Identify issues likely to be challenged by
    experienced project reviewers.

STEP 5 — SPECIALIST REVIEW

Apply the relevant reviewer perspective:

- EXECUTIVE:
  Business impact, decision usefulness, options,
  trade-offs, accountability, and major risks.

- PMO:
  Governance, document control, traceability,
  ownership, milestones, decisions, and approvals.

- TECHNICAL:
  Architecture, interfaces, assumptions, security,
  non-functional requirements, and operations.

- COMMERCIAL:
  Scope boundaries, pricing, supplier obligations,
  exclusions, acceptance, and commercial exposure.

- QA / TESTING:
  Testability, acceptance criteria, test ownership,
  environments, entry/exit criteria, and evidence.

Apply only perspectives relevant to the document.

STEP 6 — PRIORITIZE FINDINGS

Classify each issue as:

CRITICAL:
Could lead to a materially incorrect decision,
major delivery risk, or document rejection.

HIGH:
Material weakness requiring correction before issue.

MEDIUM:
Important improvement, but not necessarily blocking.

LOW:
Minor clarity, formatting, or presentation improvement.

Recommend specific corrections without inventing facts,
deadlines, owners, budgets, or contractual terms.

OUTPUT FORMAT

1. EXECUTIVE AUDIT SUMMARY

Document | Overall Quality |
Critical Findings | High Findings |
Submission Readiness

2. AUDIT FINDINGS REGISTER

Finding ID | Document Reference |
Issue | Evidence / Gap |
Why It Matters | Priority |
Recommended Correction

3. EVIDENCE AND CONSISTENCY REVIEW

Statement / Item | Classification |
Source / Evidence | Issue |
Required Validation

4. ACTION AND DECISION QUALITY

Action / Decision | Owner |
Deadline | Missing Element |
Recommended Improvement

5. TOP 3 PRIORITY CORRECTIONS

Priority | Required Correction |
Why Critical | Proposed Owner |
Evidence Required

6. REVIEWER CHALLENGE

Likely Reviewer Question |
Current Weakness | Recommended Preparation

7. QUALITY RATING

Choose:
Poor / Acceptable / Good / Excellent

Poor:
Material gaps prevent reliable use.

Acceptable:
Usable but requires significant improvement.

Good:
Generally complete with minor gaps.

Excellent:
Clear, supported, actionable,
and internally consistent.

Justify the rating in no more than three sentences.

8. SUBMISSION RECOMMENDATION

READY / READY WITH CONDITIONS / NOT READY

Explain the recommendation and identify
any remaining approval blockers.

RULES

- Audit the document; do not silently rewrite it.
- Do not invent missing information.
- Distinguish confirmed gaps from potential concerns.
- Base findings on the document and supplied evidence.
- Avoid irrelevant generic recommendations.
- Do not treat completeness as proof of accuracy.
- Do not assume AI quality ratings constitute approval.
```

### Optional Prompt — Correct and Re-Audit

Use this after validating the audit findings.

```text
ROLE

You are a Senior PMO Quality Reviewer.

INPUT

Original document: [PASTE VERSION 1]
Approved audit findings: [PASTE FINDINGS]
Revised document: [PASTE VERSION 2]

TASK

Compare the revised document with the original
and the approved audit findings.

For each finding determine:

- Resolved
- Partially Resolved
- Open
- Not Applicable

Identify:
1. Corrections successfully implemented
2. Remaining quality or governance gaps
3. New weaknesses introduced by the revision
4. Changed facts, dates, owners, risk scores,
   commitments, or decisions
5. Remaining approval blockers

OUTPUT

Finding ID | Original Issue |
Revision Made | Resolution Status |
Remaining Action

Then provide:

Updated Quality Rating
Submission Readiness
Top Remaining Corrections

Do not mark an issue resolved without evidence.
Do not treat proposed corrections as approved facts.
```

---

## 2. Quality Check

Use this prompt to evaluate whether the audit itself is reliable, relevant, and actionable.

```text
QUALITY CHECK

Act as an independent Senior Project Assurance Manager.

Review the completed Document Audit and original source.

Verify:

1. Traceability:
   Each finding references a specific document item
   or justified omission.

2. Accuracy:
   No audit finding relies on invented facts.

3. Relevance:
   Recommendations reflect the document's purpose,
   project context, and audience.

4. Materiality:
   Critical and High findings represent genuine
   governance, delivery, or decision risks.

5. Evidence:
   Unsupported claims and assumptions are clearly
   separated from verified information.

6. Actionability:
   Recommended corrections specify what is needed
   without fabricating owners or deadlines.

7. Consistency:
   Identified contradictions are accurately described.

8. Reviewer Perspective:
   Technical, commercial, QA, or executive checks
   are applied only where relevant.

9. Governance:
   The audit does not claim formal approval authority.

10. Re-Audit:
    Resolved findings are supported by revised evidence,
    and newly introduced problems are identified.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [AUDIT QUALITY ISSUES]
Required corrections: [ACTIONS]
Unsupported findings: [IF ANY]
Approval blockers: [MATERIAL GAPS]

Do not reward document length or formatting
at the expense of factual quality.
```

---

## 3. Practical IT Use Case

### CRM Implementation — Risk Register Quality Audit

**Scenario:** A Project Manager is preparing an initial risk register for a CRM implementation project. The register contains three risks, but their descriptions and mitigation actions are too general to support effective management.

Before submitting the register to the PMO, the Project Manager uses the Document Audit Workflow to identify weaknesses and develop targeted corrections.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM System Implementation |
| Document | Initial Risk Register |
| Project phase | Planning |
| Reviewer | PMO / Project Manager |
| Document purpose | Support active risk management |
| Main concern | Vague risks and weak mitigation actions |
| Management objective | Improve traceability, ownership, and risk response quality |

### Example Input

```text
Project: CRM System Implementation

Document type: Risk Register
Document version: 1.0
Project phase: Planning

RISK R-001
Description: Project delay
Likelihood: 3
Impact: 3
Mitigation: Monitor schedule

RISK R-002
Description: Cost overrun
Likelihood: 2
Impact: 4
Mitigation: Review budget monthly

RISK R-003
Description: Vendor performance
Likelihood: 3
Impact: 4
Mitigation: Manage vendor carefully

Scoring model:
Likelihood × Impact

Risk owners:
Not provided.

Risk triggers:
Not provided.

Review dates:
Not provided.
```

### Example Output — Document Audit

#### 1. Executive Audit Summary

| Area | Assessment |
|---|---|
| Document | CRM Risk Register v1.0 |
| Overall quality | Poor |
| Critical findings | 0 identified |
| High findings | 5 |
| Main weakness | Risks cannot be actively managed |
| Submission readiness | Not Ready |

**Executive assessment:** The register identifies broad risk themes but does not establish their causes, measurable triggers, accountable owners, or practical mitigation strategies.

Although risk scores can be calculated from the supplied values, the evidence supporting those assessments is not available.

#### 2. Audit Findings Register

| ID | Document Reference | Issue | Priority | Recommended Correction |
|---|---|---|---|---|
| F-01 | R-001 | Risk description too broad | High | Define cause, event, and milestone impact |
| F-02 | R-001 | Monitoring presented as mitigation | High | Define preventive action and escalation trigger |
| F-03 | R-002 | Cost driver not identified | High | Identify potential cost source and response |
| F-04 | R-003 | Supplier risk lacks specific dependency | High | Identify relevant supplier deliverable |
| F-05 | All risks | No accountable owners or triggers | High | Assign ownership and define warning indicators |
| F-06 | All risks | No review dates | Medium | Establish a risk review cadence |
| F-07 | All risks | Likelihood and impact not justified | Medium | Validate scoring against available evidence |

#### 3. Evidence and Consistency Review

| Statement / Item | Classification | Assessment |
|---|---|---|
| Project delay risk | Broad risk hypothesis | Cause not defined |
| Cost overrun risk | Broad risk hypothesis | Cost driver not identified |
| Vendor performance risk | Broad risk hypothesis | Supplier dependency not specified |
| Risk scoring | Documented assessment | Calculation possible; basis unverified |
| Mitigation measures | Proposed actions | Insufficient to reduce exposure |
| Risk ownership | Missing information | Requires assignment |

The supplied scores calculate as follows:

| Risk | Likelihood | Impact | Calculated Score |
|---|---:|---:|---:|
| R-001 | 3 | 3 | 9 |
| R-002 | 2 | 4 | 8 |
| R-003 | 3 | 4 | 12 |

These scores are arithmetically correct but must be validated against the project's risk-assessment criteria.

#### 4. Action and Decision Quality

| Current Action | Quality Gap | Recommended Improvement |
|---|---|---|
| Monitor schedule | No preventive action | Identify critical dependency and preventive measure |
| Review budget monthly | Monitoring only | Define cost driver and cost-control response |
| Manage vendor carefully | Vague and unmeasurable | Specify supplier deliverable, review evidence, and escalation condition |
| All three risks | No owner | Assign an accountable risk owner |
| All three risks | No trigger | Establish measurable early warning indicators |

**Management interpretation:** Monitoring provides visibility but does not necessarily reduce risk exposure.

#### 5. Top 3 Priority Corrections

| Priority | Correction | Why It Matters |
|---|---|---|
| 1 | Rewrite risks using cause–event–impact statements | Makes exposure specific and actionable |
| 2 | Replace generic mitigation with preventive and contingency actions | Improves management response |
| 3 | Define owners, triggers, and review dates | Establishes accountability and early escalation |

#### 6. Reviewer Challenge

| Likely PMO Question | Current Weakness | Required Preparation |
|---|---|---|
| What exactly could delay the project? | R-001 has no cause | Identify schedule dependency |
| What is driving potential cost overrun? | R-002 is generic | Identify cost exposure |
| Which supplier commitment is at risk? | R-003 lacks detail | Confirm supplier deliverable |
| Who owns these risks? | Owners missing | Assign accountability |
| When will mitigation start? | No triggers or dates | Define thresholds and review points |

#### 7. Quality Rating

**Poor**

The register provides a basic inventory of risk categories but lacks the specificity and accountability needed for active project management. The proposed mitigations describe monitoring rather than meaningful risk reduction. Significant revisions are required before formal submission.

#### 8. Submission Recommendation

**NOT READY**

Required before submission: validated risk descriptions, action-based mitigations, owners, early warning indicators, and risk-scoring rationale.

### Example Correction — Before and After

**Original Risk R-003**

```text
Risk:
Vendor performance

Likelihood: 3
Impact: 4

Mitigation:
Manage vendor carefully.
```

**Proposed Improved Risk R-003**

```text
Risk ID:
R-003

Cause:
The CRM implementation depends on a supplier-delivered
integration component.

Risk Event:
The supplier may deliver the integration component
later than the agreed testing-readiness date.

Potential Impact:
System integration testing may be delayed,
placing downstream milestones at risk.

Preventive Action:
Confirm the supplier delivery baseline and
review evidence of integration readiness
at agreed checkpoints.

Trigger:
Supplier forecast indicates that the component
will not meet the approved readiness milestone.

Contingency:
Assess testing resequencing and raise the
schedule impact through project governance.

Risk Owner:
To be assigned.

Likelihood / Impact:
Existing assessment requires validation.

Review Date:
To be agreed.
```

*This is a proposed illustration of stronger risk wording, not a confirmed CRM project risk. The supplier dependency, milestone, actions, and scoring must be checked before inclusion in the approved register.*

### Management Decisions

1. **Risk specificity:** Require each risk to identify a credible cause, event, and measurable project impact.
2. **Mitigation quality:** Distinguish preventive action from monitoring and contingency response.
3. **Accountability:** Confirm risk ownership, early warning indicators, and review frequency.
4. **Quality gate:** Re-audit the register after corrections before submitting it to the PMO.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The audit correctly identifies weaknesses in specificity, action quality, accountability, and scoring evidence. The findings are traceable to the source document, but the proposed improved risk example contains hypothetical project details requiring validation.

**Required corrections:** Confirm actual supplier dependencies and baseline dates, validate likelihood and impact assessments, assign owners, and establish review triggers.

**Approval blockers:** Unverified risk causes, missing accountable owners, and incomplete mitigation plans.

**Governance:** Supports PMI-aligned quality management, risk management, document control, project assurance, stakeholder reporting, and decision governance.

AI-assisted auditing supports professional review but does not establish document accuracy or authorize approval. Review findings must be validated by appropriate project, technical, commercial, or governance stakeholders. Protect confidential project records, financial information, contracts, security details, and sensitive stakeholder data.
