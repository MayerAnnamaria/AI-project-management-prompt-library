# Role Stacking — Author Then Reviewer

**Prompt ID:** AIWF-002 | **Category:** Advanced AI Workflows | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Improve project-management documents by challenging an initial draft from the perspective of its intended recipient, decision-maker, or specialist reviewer.

**Use case:** Review executive reports, Steering Committee papers, risk escalations, change requests, vendor communications, technical proposals, and Go / No-Go recommendations before formal submission.

Copy the master prompt, replace the placeholders, and execute the stages sequentially.

### Master Prompt — Author and Reviewer Workflow

```text
ROLE

You are an experienced IT Project Manager and independent
project assurance specialist.

You will perform three distinct roles:

1. AUTHOR — Create the initial document.
2. REVIEWER — Challenge it from the recipient's perspective.
3. EDITOR — Address validated findings and prepare
   the final document.

Keep these roles separate.

CONTEXT

Project: [PROJECT NAME]
Document type: [STATUS REPORT / DECISION PAPER / OTHER]
Project phase: [PHASE]
Delivery approach: [PREDICTIVE / AGILE / HYBRID]

Intended recipient: [SPONSOR / STEERING COMMITTEE /
CFO / CTO / CISO / PRODUCT OWNER / OTHER]

Document objective: [PURPOSE]
Decision required: [IF APPLICABLE]
Approved project facts: [PASTE VERIFIED INFORMATION]
Known assumptions: [LIST]
Relevant constraints: [LIST]
Required approval authority: [ROLE / NOT PROVIDED]

TASK

STAGE 1 — AUTHOR

Act as a Senior IT Project Manager.

Create a concise, professional document using only
the supplied project information.

Ensure the draft clearly explains:

1. Current situation or business problem
2. Supporting facts and evidence
3. Material project impact
4. Risks and dependencies
5. Actions taken or proposed
6. Decisions or support required

Distinguish confirmed facts from forecasts,
assumptions, and recommendations.

OUTPUT

Draft Document — Version 1
Information Gaps

Stop after Stage 1 for review.

STAGE 2 — RECIPIENT REVIEW

Switch roles.

Act as [REVIEWER ROLE], receiving the document
for review or decision-making.

Challenge the draft independently.

Assess:

1. Does the document address your main concerns?
2. Are important claims supported by evidence?
3. Is business or operational impact clear?
4. Are risks, assumptions, and trade-offs transparent?
5. Is ownership and accountability defined?
6. Are decisions and deadlines explicit?
7. What information would prevent approval?
8. What five questions would you ask the author?

Do not automatically agree with the author's conclusions.

OUTPUT

Reviewer Assessment
Three Most Material Weaknesses
Five Likely Reviewer Questions
Missing Evidence
Recommended Improvements

Stop after Stage 2.

STAGE 3 — REVISION AND RECONCILIATION

Return to the Senior IT Project Manager role.

Review the recipient's findings.

1. Correct substantiated weaknesses.
2. Clarify business impact and decision requirements.
3. Incorporate verified additional information.
4. Preserve factual accuracy and original commitments.
5. Identify unresolved evidence gaps.
6. Distinguish competing stakeholder perspectives
   where relevant.
7. Produce a concise, decision-ready final version.

Do not invent information to satisfy reviewer questions.

OUTPUT

Final Revised Document — Version 2

REVIEW RECONCILIATION

Reviewer Finding | Correction Made |
Supporting Evidence | Remaining Gap

FINAL MANAGEMENT SUMMARY

- Main improvement
- Unresolved questions
- Decision readiness
- Required human review

RULES

- Do not invent project facts, metrics, or approvals.
- Do not assume the simulated reviewer represents
  a real stakeholder's actual opinion.
- Do not treat AI role-play as formal sign-off.
- Preserve material facts during revision.
- Highlight disagreements rather than forcing consensus.
- Escalate legal, financial, security, or contractual
  questions to authorized specialists.
```

### Optional — Multi-Reviewer Challenge

Use this variation for high-impact or cross-functional decisions.

```text
MULTI-REVIEWER CHALLENGE

Review the document below from three independent perspectives.

DOCUMENT

[PASTE DOCUMENT]

REVIEWERS

1. [REVIEWER A]
2. [REVIEWER B]
3. [REVIEWER C]

For each reviewer:

- Identify the primary objective.
- Challenge the three most material weaknesses.
- Identify missing evidence.
- Explain relevant risks and concerns.
- Recommend necessary corrections.

Then reconcile the findings.

OUTPUT

Reviewer | Main Concern |
Evidence Required | Risk | Recommendation

CROSS-REVIEWER RECONCILIATION

Areas of Agreement
Conflicting Priorities
Unresolved Trade-Offs
Decision Options
Required Human Approvals

Do not imply that reviewers have agreed
or approved the document.
```

### Reviewer Selection Guide

Choose reviewers according to the actual document and its intended audience.

| Reviewer | Primary Focus | Suitable Documents |
|---|---|---|
| Executive Sponsor | Business value, delivery confidence, decisions | Status reports, executive updates |
| Steering Committee | Options, trade-offs, governance | Decision papers, escalations |
| CFO / Finance | Cost, forecast, contingency, financial exposure | Business cases, budget changes |
| CTO / Architect | Technical feasibility, architecture, dependencies | Technical proposals |
| CISO / Security | Security controls, vulnerabilities, approval evidence | Go-live and security assessments |
| Product Owner | Business value, requirements, acceptance | Product and scope documents |
| Operations / Service Manager | Supportability, monitoring, handover | Release readiness |
| Supplier Delivery Manager | Delivery commitments, responsibilities, evidence | Vendor escalations |
| Procurement / Commercial | Contract, pricing, assumptions, change control | Supplier assessments, variations |
| PMO | Consistency, ownership, dates, traceability | Risk registers, status reports |
| End User | Clarity, user impact, required actions, support | Change notifications |

For material decisions, choose the two or three perspectives most likely to expose different risks. Additional reviewers should provide distinct value rather than duplicate the same checks.

---

## 2. Quality Check

Use this independent quality gate after the author/reviewer process.

```text
QUALITY CHECK

Act as an independent Senior PMO Quality Assurance Manager.

Review:

- Original document
- Reviewer findings
- Final revised document
- Available supporting evidence

VERIFY

1. ROLE SEPARATION

The reviewer challenged the draft independently
rather than simply endorsing its conclusions.

2. EVIDENCE

Material claims are supported by project evidence.

3. RELEVANCE

Reviewer concerns reflect the actual document
purpose and recipient's responsibilities.

4. FACTUAL INTEGRITY

The revision preserves verified dates, financial data,
risk positions, commitments, and project status.

5. DECISION READINESS

Required decisions, options, consequences,
and approval authority are visible.

6. REVIEWER CHALLENGE

Important assumptions, weak evidence,
and alternative interpretations are identified.

7. CONFLICT MANAGEMENT

Different reviewer priorities are documented
rather than artificially reconciled.

8. CORRECTIVE ACTION

Each material finding is addressed or explicitly
recorded as unresolved.

9. GOVERNANCE

Simulated specialist reviews are not represented
as actual stakeholder approval.

10. COMMUNICATION QUALITY

The final document is concise, professional,
audience-specific, and actionable.

OUTPUT

Quality Verdict: PASS / REVISE

FINDINGS TABLE

Finding | Evidence |
Project Impact | Correction Required |
Priority

REVIEW RECONCILIATION

Reviewer Concern | Status |
Correction | Outstanding Information

FINAL ASSESSMENT

Decision Readiness:
READY / READY WITH CONDITIONS / NOT READY

Approval Blockers:
[LIST]

Required Human Review:
[ROLES]

Do not invent evidence, stakeholder opinions,
or approvals to complete the assessment.
```

---

## 3. Practical IT Use Case

### Enterprise CRM Replacement — Executive Status Review

**Scenario:** A CRM replacement project is experiencing a testing dependency delay. The Project Manager must inform the Executive Sponsor that UAT is forecast to start five working days late while the planned production release remains achievable, although schedule contingency has reduced.

The first draft explains the problem and recovery measures. The simulated Executive Sponsor then challenges whether the report contains enough evidence to support management decisions.

### Project Context

| Attribute | Details |
|---|---|
| Project | Enterprise CRM Replacement |
| Document | Executive Project Status Update |
| Delivery approach | Hybrid |
| Overall status | Amber |
| Main dependency | External identity-provider certification |
| UAT forecast | Five working days late |
| Release outlook | Currently achievable, with reduced contingency |
| Recovery actions | Mock authentication, test resequencing, vendor escalation |
| Recipient | Executive Sponsor |
| Management objective | Communicate delivery exposure and decision requirements |

### Example Input

```text
PROJECT
Enterprise CRM Replacement

OVERALL STATUS
Amber

CURRENT SITUATION
UAT is forecast to start five working days late
because external identity-provider certification
remains incomplete.

ACTIONS TAKEN
- Mock authentication service implemented.
- Unaffected testing activities resequenced.
- Vendor escalation active.

BUSINESS IMPACT
The current production release date remains
achievable, but schedule contingency has reduced.

DECISION REQUIRED
Not provided.

REMAINING CONTINGENCY
Not quantified.

CERTIFICATION COMPLETION FORECAST
Not provided.
```

### Stage 1 — Author: Initial Executive Update

**Executive Project Status — Amber**

The Enterprise CRM Replacement project remains Amber because external identity-provider certification is incomplete, resulting in a forecast five-working-day delay to the start of UAT.

The project team has implemented a mock authentication service, re-sequenced unaffected testing activities, and escalated the dependency to the vendor.

The planned production release remains achievable, although schedule contingency has reduced.

The team continues to monitor certification progress and its impact on downstream testing activities.

### Stage 2 — Reviewer: Executive Sponsor Challenge

The Executive Sponsor reviews the update from the perspective of delivery confidence, business impact, accountability, and decision requirements.

#### Reviewer Assessment

| Weakness | Executive Concern | Recommended Improvement |
|---|---|---|
| Release confidence unsupported | Why is the planned release still achievable? | Provide evidence of remaining contingency and recovery feasibility |
| Certification deadline unclear | When must the dependency be resolved? | Confirm supplier forecast and latest acceptable completion date |
| No explicit decision required | What action is expected from the Sponsor? | State any required escalation or decision, or confirm none currently requested |

#### Five Likely Sponsor Questions

1. How much schedule contingency remains after the forecast UAT delay?
2. What evidence supports the statement that production release remains achievable?
3. When is the supplier expected to complete certification?
4. What alternative delivery options exist if certification is delayed further?
5. What decision or intervention would be required from the Sponsor, and by when?

**Reviewer conclusion:** The update communicates the immediate problem but does not provide enough evidence to establish release confidence or identify a specific executive decision.

### Stage 3 — Project Manager: Revised Executive Update

**Enterprise CRM Replacement — Executive Status: Amber**

UAT is forecast to start **five working days late** because external identity-provider certification remains incomplete.

The project team has implemented mock authentication, re-sequenced unaffected testing, and escalated the outstanding certification to the supplier.

The current production release remains the planning target. However, schedule contingency has reduced, and available information does not yet quantify the remaining buffer or establish a confirmed certification completion date.

**Management attention required:** Obtain the supplier's confirmed certification forecast, assess the remaining schedule contingency, and determine whether additional executive intervention is needed.

**Decision status:** No specific Sponsor decision has yet been defined. The Project Manager must clarify the decision or escalation requirement before formal submission.

### Review Reconciliation

| Reviewer Finding | Revision Made | Remaining Gap |
|---|---|---|
| Release confidence unsupported | Qualified the release outlook | Quantified contingency and forecast evidence |
| Supplier completion unclear | Made dependency uncertainty explicit | Confirmed supplier completion date |
| Executive decision unclear | Added management attention required | Formal decision, authority, and deadline |

The revised version is stronger because it makes uncertainty visible instead of presenting unsupported confidence.

### Example — Multi-Reviewer Go / No-Go Challenge

For a more consequential decision, role stacking can involve several reviewers with distinct responsibilities.

**Illustrative readiness inputs:**

| Readiness Area | Reported Status |
|---|---|
| UAT | Complete |
| Critical defects | 0 |
| High-severity defects | 2, with approved workarounds |
| Security | Approved |
| Migration rehearsal | Passed |
| Operations runbook | Approved |
| Vendor support | Confirmed |
| User training | 95% complete |

These inputs do not independently establish that production release is authorized.

| Reviewer | Main Challenge | Evidence Required |
|---|---|---|
| CISO | Do the two high-severity defects introduce security exposure? | Defect classification and security evidence |
| Service Manager | Can Operations support the solution and handle known issues? | Handover, monitoring, and incident procedures |
| Executive Sponsor | Is the remaining business risk acceptable? | Impact assessment, alternatives, and accountable recommendation |

**Potential conflict:** Security may require additional evidence, Operations may consider the service supportable, and the Sponsor may prioritize the committed release date.

The Project Manager should document these differences and present the decision options. AI should not force simulated reviewers into agreement.

### Management Decisions

1. **Strengthen release confidence:** Require evidence supporting schedule feasibility rather than relying solely on an optimistic forecast.
2. **Clarify accountability:** Obtain supplier commitments, remaining dependency dates, and appropriate escalation ownership.
3. **Improve decision readiness:** Ensure the Executive Sponsor understands the business impact, unresolved risks, and any required intervention.
4. **Preserve reviewer independence:** Document conflicting specialist perspectives and refer material decisions to authorized stakeholders.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The role-stacking process exposed gaps in schedule evidence, supplier commitments, and executive decision clarity. The revised report communicates those uncertainties without introducing unsupported project facts.

**Required corrections:**
- Confirm remaining schedule contingency.
- Obtain a validated supplier certification forecast.
- Assess the downstream impact of the delayed UAT start.
- Establish whether a Sponsor decision is required.
- Validate release assumptions before formal reporting.

**Approval blockers:** Incomplete schedule evidence and an undefined executive decision or escalation requirement.

**Governance:** Supports PMI-aligned stakeholder management, quality assurance, project communications, risk management, decision-making, and governance.

### Professional Use and Limitations

Role stacking helps anticipate stakeholder questions, identify competing priorities, and improve document quality. It does not reproduce the real views of an individual reviewer or substitute for specialist judgment.

AI acting as a CISO does not provide security approval. AI acting as legal counsel does not replace authorized legal review. Financial, commercial, operational, and delivery decisions remain with the relevant decision authorities.

For confidential documents, follow organizational AI-use policies and protect sensitive project information, supplier pricing, technical architecture, contract terms, and security details.
