# Contractual Claim / Formal Notification

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** COMM-002 | **Category:** Commercial & Project Governance

---


## 1. Ready-to-Use Prompt

**Purpose:** Prepare factual, evidence-based contractual notifications that document delivery events, potential impacts, mitigation measures, and requested actions for commercial and legal review.

**Use case:** Draft formal notifications when delayed dependencies, unavailable environments, missed approvals, scope changes, or supplier performance issues may affect contractual commitments.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager and Commercial Management
Specialist experienced in software implementation, supplier
contracts, change control, contractual correspondence,
and project governance.

CONTEXT

Project: [PROJECT NAME]
Contract / version: [NAME / VERSION]
Contract type: [SOFTWARE / SAAS / CLOUD / OUTSOURCING / OTHER]
Customer: [PARTY]
Supplier: [PARTY]
Current phase: [PHASE]
Delivery approach: [PREDICTIVE / AGILE / KANBAN / HYBRID]

Relevant contractual clauses: [PASTE EXACT WORDING]
Notice requirements: [PASTE VERIFIED REQUIREMENTS]
Authorized notice sender: [ROLE / UNKNOWN]
Contractual recipient: [ROLE / UNKNOWN]
Required delivery method: [METHOD / UNKNOWN]

EVENT DETAILS

Event: [DESCRIPTION]
Contractual / planned commitment: [DETAILS]
Original required date: [DATE]
Actual date / current status: [DETAILS]
Date event occurred: [DATE]
Date project became aware: [DATE]
Previous notices: [DETAILS / NONE]

IMPACT AND EVIDENCE

Schedule impact: [DETAILS]
Cost / resource impact: [DETAILS]
Scope / quality impact: [DETAILS]
Affected dependencies: [LIST]
Potential concurrent causes: [IF RELEVANT]
Supporting evidence: [LIST]
Mitigation already implemented: [LIST]
Remaining recovery actions: [LIST]

REQUESTED OUTCOME

Action / relief requested: [DETAILS]
Response deadline: [DATE / UNKNOWN]
Commercial / legal review status: [STATUS]

TASK

Prepare a factual contractual notification draft and
identify the checks required before formal issuance.

STEP 1 — VERIFY CONTRACTUAL REQUIREMENTS

1. Identify relevant clauses and their explicit requirements.
2. Extract notice triggers, periods, recipients, delivery
   methods, and required supporting information.
3. Verify event, awareness, and notice dates.
4. Flag missing contractual wording, definitions,
   or notice requirements for Legal review.
5. Do not infer entitlement or contractual breach
   from the occurrence of a project delay alone.

STEP 2 — DOCUMENT EVENT AND IMPACT

6. Describe the event using verified facts and chronology.
7. Distinguish:
   - Planned commitments
   - Actual events
   - Confirmed impacts
   - Forecast impacts
   - Unverified assumptions
8. Link the event to affected activities and dependencies.
9. Assess schedule, cost, resource, scope, and quality
   impacts only where evidence exists.
10. Identify potential concurrent causes or alternative
    explanations requiring investigation.
11. Document mitigation and recovery actions already taken.

STEP 3 — PREPARE FORMAL COMMUNICATION

12. Draft a precise, professional notification containing:
    - Subject and reference
    - Purpose of notice
    - Verified contractual basis
    - Factual event description
    - Chronology
    - Supported project impact
    - Mitigation actions
    - Action or relief requested
    - Supporting evidence
    - Next steps and professional close
13. State the requested response and deadline clearly.
14. Identify whether the matter requires formal change control.
15. Include reservations of rights or legal wording only
    when supplied or approved by qualified Legal counsel.

STEP 4 — VALIDATE BEFORE ISSUE

16. Challenge the draft from the counterparty's perspective.
17. Identify missing evidence, disputed causation,
    chronology gaps, and unsupported assertions.
18. Prepare a notice-tracking record.
19. List required commercial and legal approvals.
20. Recommend follow-up actions after issuance.

RULES

- Do not invent contractual rights, remedies,
  notice periods, clauses, liability, or damages.
- Do not present a forecast as a confirmed impact.
- Distinguish delays to individual activities from
  delays to the overall project or critical path.
- Do not assume that a notification automatically
  approves a change request or commercial claim.
- Use formal, neutral, precise, non-adversarial language.
- Mark missing legal or contractual requirements
  as "Requires verification".

OUTPUT FORMAT

1. FORMAL NOTIFICATION DRAFT

Subject: [EVENT AND PROJECT REFERENCE]

Dear [AUTHORIZED RECIPIENT],

[Purpose and verified contractual basis]

[Factual description and chronology]

[Current and forecast project impact]

[Mitigation and recovery actions]

[Explicit request and response deadline]

[Supporting evidence and next steps]

Kind regards,
[AUTHORIZED SENDER]

2. EVENT CHRONOLOGY

Date | Event | Supporting Evidence |
Confirmed / Unverified

3. IMPACT AND CAUSATION REVIEW

Affected Activity | Event / Cause |
Confirmed Impact | Forecast Impact |
Evidence | Alternative Causes

4. SUPPORTING EVIDENCE REGISTER

Evidence ID | Document / Record |
Date | Relevance | Availability

5. CONTRACTUAL NOTICE CHECK

Requirement | Contract Reference |
Verified Position | Gap / Required Action

Include:
- Notice trigger and deadline
- Recipient and authorized sender
- Delivery method
- Supporting documents
- Receipt / delivery evidence

6. CLAIM AND CHANGE-CONTROL FOLLOW-UP

Action | Proposed Owner | Deadline |
Required Evidence | Approval / Decision

7. MANAGEMENT SUMMARY

- Verified event and current impact
- Potential contractual significance
- Evidence and causation gaps
- Required legal / commercial review
- Issuance readiness and next steps

Use concise Markdown tables.
Clearly distinguish draft wording from approved notices.
```

---

## 2. Quality Check

Run this independent review before any formal notification is issued.

```text
QUALITY CHECK

Act as an independent Senior Commercial Assurance
and QA Manager reviewing a contractual notification.

Review the draft against the contract and project evidence.

Verify:

1. Contractual Accuracy:
   Clauses, obligations, notice conditions, and recipients
   are supported by the supplied agreement.

2. Timing:
   Event date, awareness date, notice period, deadline,
   and delivery requirements are verified.

3. Evidence:
   Statements are supported by contemporaneous records,
   with missing documents identified.

4. Causation:
   The event is linked to specific project impacts.
   Concurrent causes and alternative explanations
   have been considered.

5. Commercial Accuracy:
   Costs, delays, and requested relief are supported
   or explicitly marked as provisional.

6. Mitigation:
   Recovery actions and their actual effects
   are represented accurately.

7. Communication:
   The tone is formal, precise, factual,
   and free from unsupported allegations.

8. Governance:
   Required Legal / Commercial approval and
   change-control procedures are identified.

9. Counterparty Review:
   Likely objections, evidence gaps, and
   disputed assumptions are highlighted.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Counterparty Challenges: [POTENTIAL OBJECTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not infer entitlement, liability, contractual breach,
or legal effect without qualified professional review.

Do not declare a notice valid or timely without
verified contractual requirements.
```

---

## 3. Practical IT Use Case

### CRM Implementation — Delayed Integration Environment

**Scenario:** A software supplier is implementing a CRM system. The customer-provided integration environment becomes available later than planned, delaying end-to-end testing and potentially affecting UAT.

The Project Manager must document the event, preserve relevant evidence, and prepare a notification for Commercial and Legal review.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM System Implementation |
| Phase | System Integration Testing |
| Contract | Software Implementation Agreement |
| Event | Delayed integration environment |
| Planned availability | 10 May 2027 |
| Actual availability | 24 May 2027 |
| Reported testing impact | 10 working days |
| Forecast UAT impact | 5 working days |
| Requested outcome | Event acknowledgment and schedule impact review |
| Governance requirement | Verified notice procedure and formal change control |

### Example Input

```text
Project: CRM System Implementation

Contract: Software Implementation Agreement
Customer: CRM Implementation Customer
Supplier: CRM Implementation Vendor

Relevant clause:
Clause 8.3 — Customer Dependencies

Exact clause wording:
Not provided.

Reported notice requirement:
Written notification within 10 business days
of becoming aware of a dependency delay.

Event:
Production-equivalent integration environment
was provided later than planned.

Required availability: 10 May 2027
Actual availability: 24 May 2027
Awareness date: Not confirmed

Reported impact:
- Integration testing started 10 working days late.
- Forecast UAT delay: 5 working days.
- Additional cost: Under assessment.

Mitigation:
- Mock services used for eligible testing.
- Unaffected activities re-sequenced.

Evidence:
- Approved project schedule
- Environment request log
- Project meeting minutes
- Environment access confirmation

Requested action:
Customer acknowledgment and formal review
of the proposed schedule adjustment.

Legal review:
Not yet completed.
```

### Example Output — Contractual Notification Package

#### 1. Formal Notification Draft

**Subject: CRM Implementation — Notification of Delayed Integration Environment Availability**

Dear [Authorized Customer Representative],

We are writing to record the delayed availability of the production-equivalent integration environment required for the CRM implementation project.

According to the current project records, the environment was planned to be available on 10 May 2027 but became accessible on 24 May 2027.

The project team reports that this affected the start of end-to-end integration testing by ten working days. Following the use of mock services and re-sequencing of unaffected activities, the current project forecast indicates a potential five-working-day impact on UAT.

The team is continuing recovery activities to minimize downstream disruption. We request acknowledgment of the reported event and a joint review of the resulting schedule impact through the applicable project change-control process.

Supporting evidence includes the approved schedule, environment request history, meeting records, and access confirmation.

Please confirm the appropriate representative and proposed review arrangements so that the schedule assessment can be progressed.

Kind regards,  
[Authorized Supplier Representative]

*Draft status: For Commercial and Legal review only. The contractual clause wording, notice deadline, recipient, and issuance method must be verified before this draft is treated as a formal contractual notice.*

#### 2. Event Chronology

| Date | Event | Evidence | Status |
|---|---|---|---|
| 10 May 2027 | Planned environment availability | Approved schedule | Reported |
| TBD | Delay identified by project team | Request log / minutes | Requires verification |
| 24 May 2027 | Environment access provided | Access confirmation | Reported |
| TBD | Recovery and impact assessment | Updated schedule | Requires validation |

#### 3. Impact and Causation Review

| Area | Current Assessment | Evidence Required |
|---|---|---|
| Environment | Available 14 calendar days after planned date | Access log |
| Integration testing | Started 10 working days later than planned | Test schedule / execution record |
| UAT | Forecast five-working-day impact | Dependency and recovery analysis |
| Cost | Under assessment | Timesheets / cost records |
| Mitigation | Mock services and re-sequencing reported | Test and planning records |
| Concurrent causes | Not assessed | Defect, resource, and schedule history |

**Management concern:** A late environment does not automatically establish the same amount of delay to the overall project. The downstream impact requires a defensible dependency and recovery analysis.

#### 4. Supporting Evidence Register

| ID | Evidence | Relevance | Availability |
|---|---|---|---|
| E-01 | Approved schedule | Baseline environment date | Referenced |
| E-02 | Environment request log | Requests and timing | Referenced |
| E-03 | Meeting minutes | Awareness and escalation history | Referenced |
| E-04 | Access confirmation | Actual availability date | Referenced |
| E-05 | Updated project forecast | Claimed UAT impact | Not provided |
| E-06 | Resource / cost evidence | Potential additional cost | Not provided |

A referenced document must be checked before it is treated as verified evidence.

#### 5. Contractual Notice Check

| Requirement | Current Position | Required Action |
|---|---|---|
| Contract clause | Clause 8.3 reported | Review exact wording |
| Notice trigger | Environment delay | Verify contractual definition |
| Awareness date | Unknown | Confirm from records |
| Notice period | Reported as 10 business days | Verify wording and calculation |
| Recipient | Unknown | Confirm contractual notice recipient |
| Delivery method | Unknown | Check notice provisions |
| Authorized sender | Unknown | Confirm delegated authority |
| Delivery evidence | Not available | Retain proof after issuance |

**Issuance readiness: Not confirmed.**

The notice deadline cannot be reliably determined without the awareness date, verified contract provisions, and applicable business-day rules.

#### 6. Claim and Change-Control Follow-Up

| Action | Proposed Owner | Timing | Required Evidence |
|---|---|---|---|
| Verify Clause 8.3 and notice provisions | Legal / Commercial Manager | Before issuance | Contract extract |
| Confirm awareness date | Project Manager | Before deadline calculation | Event records |
| Validate testing and UAT impacts | Project Planner / Test Lead | Before impact submission | Schedule analysis |
| Assess additional costs | Commercial Manager | Before any cost claim | Financial evidence |
| Approve notification wording | Authorized Legal / Commercial reviewer | Before issuance | Reviewed draft |
| Track notice issuance | Contract Administrator | On authorized issuance | Delivery confirmation |
| Process schedule adjustment | Project Manager | After impact review | Change-control decision |

### Management Decisions

1. **Notice compliance:** Verify the contract's notice requirements and applicable deadline immediately.
2. **Evidence:** Confirm event chronology and support the reported testing delay with project records.
3. **Commercial position:** Assess whether additional cost or schedule relief may be available, without assuming entitlement.
4. **Governance:** Obtain Legal and Commercial approval before formal issuance and manage any proposed baseline change through authorized change control.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The draft presents the reported event, project impact, mitigation actions, and requested review in a factual, non-adversarial manner. However, the exact contractual basis, awareness date, authorized recipient, notice method, and causation evidence are incomplete.

**Required corrections:** Verify contract wording and notice timing; validate schedule effects and supporting records; assess possible concurrent causes; obtain authorized review before issuance.

**Counterparty challenges:** Whether the environment delay caused the entire testing delay, whether the UAT forecast reflects all contributing factors, and whether the notice complies with contractual procedures.

**Approval blockers:** Unverified notice requirements, unknown awareness date, and missing Legal / Commercial authorization.

**Governance:** Supports PMI-aligned procurement administration, schedule management, change control, risk management, documentation, and stakeholder communication.

A contractual notification does not itself establish entitlement, liability, or approval of a change. Formal notices and claims require authorized commercial and legal review. Protect confidential contract provisions, pricing, dispute strategy, security information, and customer data.
