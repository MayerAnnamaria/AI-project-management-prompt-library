# Steering Committee Decision Paper

**Prompt ID:** REPORT-003 | **Category:** Reporting & Communication | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Present evidence-based options, trade-offs, and recommendations to support timely steering committee decisions on material project issues.

**Use case:** Request governance approval for changes to project funding, schedule, scope, resources, or delivery approach when decisions exceed the Project Manager's authority.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software
delivery, executive governance, financial decision-making,
risk management, and stakeholder communication.

CONTEXT

Project: [PROJECT NAME]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target milestone: [DATE]
Overall RAG status: [GREEN / AMBER / RED / UNKNOWN]

Decision required: [SPECIFIC APPROVAL / DIRECTION]
Current issue: [DESCRIPTION]
Verified facts: [EVIDENCE]
Business impact: [SCHEDULE / COST / SCOPE / QUALITY]
Actions already taken: [LIST]
Decision deadline: [DATE]
Impact if delayed: [CONSEQUENCE]
Decision authority: [ROLE / GOVERNANCE BODY]
Constraints and dependencies: [LIST]

OPTIONS

Option A: [DESCRIPTION]
Cost impact: [AMOUNT / ESTIMATE]
Schedule impact: [DETAILS]
Scope / quality impact: [DETAILS]
Risks and benefits: [DETAILS]

Option B: [DESCRIPTION]
Cost impact: [AMOUNT / ESTIMATE]
Schedule impact: [DETAILS]
Scope / quality impact: [DETAILS]
Risks and benefits: [DETAILS]

Additional options: [IF APPLICABLE]
PM recommendation: [OPTION / NOT YET DETERMINED]
Supporting evidence: [REPORTS / FORECASTS / ASSESSMENTS]

TASK

Prepare a concise Steering Committee Decision Paper.

1. State the exact decision required and why governance
   approval is necessary.
2. Summarize the issue, verified facts, actions taken,
   and current project impact.
3. Explain why the decision is time-sensitive.
4. Compare realistic, actionable options consistently across:
   - Cost and funding
   - Schedule and milestones
   - Scope and quality
   - Business value
   - Risk and dependencies
   - Implementation feasibility
5. Distinguish confirmed facts, estimates, assumptions,
   and unresolved information gaps.
6. Challenge unrealistic options and unsupported benefits.
7. Recommend the preferred option using evidence,
   business value, and explicit trade-offs.
8. State residual risks and conditions for implementation.
9. Specify the decision owner, deadline, and consequence of delay.
10. Define implementation actions following approval.
11. Identify supporting attachments and required follow-up
    in the project Decision Log.

For Agile projects, escalate only decisions beyond normal
Product Owner or delivery-team authority.

Do not invent cost estimates, schedule recovery,
contractual obligations, or approvals.

If evidence is insufficient for a firm recommendation,
identify what must be validated before approval.

OUTPUT FORMAT

1. DECISION SUMMARY

Decision Required | Recommended Option |
Decision Authority | Deadline | Impact if Delayed

2. BACKGROUND AND DECISION CONTEXT

Issue | Verified Facts | Current Impact |
Actions Taken | Why Governance Approval Is Required

3. OPTIONS COMPARISON

Option | Cost Impact | Schedule Impact |
Scope / Quality Impact | Business Benefit |
Key Risk | Feasibility

4. RISK, ASSUMPTIONS, AND TRADE-OFFS

Option | Confirmed Evidence | Assumptions |
Dependencies | Residual Exposure

5. PROJECT MANAGER RECOMMENDATION

Preferred Option | Supporting Rationale |
Main Trade-Off | Conditions | Remaining Risk

6. FORMAL DECISION REQUEST

Approval Requested | Decision Owner |
Deadline | Funding / Authority Required

7. IMPLEMENTATION ACTIONS

Action | Proposed Owner | Due Date |
Dependency | Expected Outcome

8. SUPPORTING EVIDENCE

Document | Relevance | Availability

9. DECISION LOG ENTRY

Decision ID | Decision | Date | Approver |
Conditions | Follow-Up | Status

Use concise Markdown tables and executive-level language.
Mark unapproved decisions as "Pending".
Keep the main decision paper suitable for a short governance review.
```

---

## 2. Quality Check

Use this independent review before distributing the decision paper.

```text
QUALITY CHECK

Act as a Senior PMO Director reviewing a Steering Committee
Decision Paper.

Verify:

1. Clarity: The requested decision and authority are explicit.
2. Evidence: Facts, estimates, assumptions, and information
   gaps are distinguished.
3. Options: Alternatives are realistic and compared fairly.
4. Financials: Cost estimates are supported and comparable.
5. Schedule: Milestone impacts and recovery assumptions
   are defensible.
6. Risk: Material trade-offs, dependencies, and residual
   exposure are visible.
7. Recommendation: The preferred option is supported
   by business value and evidence, not bias.
8. Governance: Deadline, approval authority,
   implementation ownership, and follow-up are defined.

Challenge whether maintaining the current approach
is a legitimate alternative.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent evidence, budgets, commitments, or approvals.
```

---

## 3. Practical IT Use Case

### Software Development — QA Capacity vs. Release Delay

**Scenario:** A software team is preparing a reporting enhancement for production. Regression testing is behind schedule because two critical defects required additional investigation and retesting.

The Project Manager must seek a governance decision on whether to fund temporary QA support or revise the release schedule.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Phase | Regression Testing |
| Delivery approach | Hybrid |
| Planned release | 30 September 2027 |
| Current status | Amber |
| Key issue | Regression testing behind schedule |
| Decision authority | Project Steering Committee |
| Decision required | Additional QA capacity or release delay |

### Example Input

```text
Project: Web Application Reporting Enhancement

Phase: Regression Testing
Target release: 30 September 2027
Overall status: Amber

Current issue:
Regression testing is five working days behind plan.

Cause:
Additional investigation and retesting of two
critical defects required unplanned QA effort.

Current impact:
The original test completion milestone is at risk.

Option A — Maintain Existing Capacity:
- No additional staffing cost.
- Forecast release delay: 1 week.
- Lower onboarding and coordination effort.
- Business launch delayed.

Option B — Add Temporary QA Capacity:
- Proposed additional cost: €12,000.
- Two QA engineers for three weeks.
- Potential recovery: 3–5 working days.
- Recovery depends on onboarding and defect readiness.

Business constraint:
September release is preferred but not contractually fixed.

Recommendation:
Option B, subject to capacity and recovery validation.

Decision deadline:
15 September 2027.

Decision authority:
Steering Committee.
```

### Example Output — Steering Committee Decision Paper

#### 1. Decision Summary

| Field | Decision Requirement |
|---|---|
| Decision required | Approve additional QA capacity or accept a revised release date |
| Recommended option | B — Temporary QA support, conditional |
| Funding requested | Up to €12,000 |
| Decision authority | Steering Committee |
| Deadline | 15 September 2027 |
| Impact if delayed | Reduced time to mobilize resources and recover testing |

#### 2. Background and Decision Context

Regression testing is five working days behind the original plan following additional investigation and retesting of two critical defects.

The release remains targeted for 30 September, but the existing testing capacity may not support completion within the current schedule.

The Project Manager requires Steering Committee direction because the preferred recovery approach involves additional project expenditure.

#### 3. Options Comparison

| Criterion | Option A — Accept Delay | Option B — Add QA Capacity |
|---|---|---|
| Additional staffing cost | €0 | €12,000 estimated |
| Schedule impact | Forecast one-week delay | Potential recovery of 3–5 working days |
| Scope | Unchanged | Unchanged |
| Quality | Existing testing approach | Additional test capacity |
| Main benefit | Avoids additional staffing cost | Opportunity to protect release |
| Main risk | Delayed business launch | Recovery not guaranteed |
| Feasibility | Dependent on revised release approval | Dependent on resource availability |

**Assessment:** Option A is financially conservative. Option B may better protect the planned release but introduces cost and execution uncertainty.

#### 4. Risk, Assumptions, and Trade-Offs

| Area | Option A | Option B |
|---|---|---|
| Schedule | Later release likely | Recovery possible but uncertain |
| Cost | No additional staffing cost assumed | €12,000 estimated |
| Quality | Testing time can be preserved through delay | Testing coverage must remain unchanged |
| Dependencies | Approval of revised release | QA availability, onboarding, test readiness |
| Residual risk | Business launch delay | Incomplete schedule recovery |

**Information gaps:** Availability of qualified QA engineers, realistic onboarding time, remaining test effort, and whether critical defects are ready for retesting.

#### 5. Project Manager Recommendation

**Recommend Option B — Temporary QA Capacity, subject to validation.**

The proposed investment provides an opportunity to protect the September release while maintaining the planned testing scope.

Approval should be conditional on confirming that the additional engineers can contribute within the remaining schedule and that the recovery forecast is technically credible.

**Main trade-off:** Additional cost in exchange for potential schedule recovery.

**Residual risk:** The planned release may still be delayed if critical fixes or remaining tests cannot be completed.

#### 6. Formal Decision Request

The Steering Committee is requested to approve **up to €12,000 for two temporary QA engineers for three weeks**, conditional on:

- Confirmed resource availability and onboarding feasibility.
- Validated remaining regression effort.
- An updated testing and release forecast.
- Continued compliance with release quality criteria.

**Decision deadline:** 15 September 2027.

Decision status: **Pending approval**.

#### 7. Implementation Actions

| Action | Proposed Owner | Due Date | Expected Outcome |
|---|---|---|---|
| Validate QA availability and rates | Project Manager | Before approval | Confirm resource feasibility |
| Confirm remaining test effort | QA Lead | Before approval | Validate recovery assumptions |
| Mobilize approved QA resources | Resource Manager | After approval | Additional testing capacity |
| Update test schedule | QA Lead | After mobilization | Revised completion forecast |
| Review release readiness | Project Manager / QA Lead | Before go/no-go | Evidence-based release decision |

#### 8. Supporting Evidence

| Document | Relevance | Availability |
|---|---|---|
| Regression test report | Remaining testing and defects | Requires validation |
| Project schedule | Baseline and recovery forecast | Referenced in scenario |
| QA resource proposal | Capacity and cost | Requires confirmation |
| Risk register | Residual release exposure | Not provided |
| Budget forecast | Funding implications | Not provided |

#### 9. Decision Log Entry

| Field | Value |
|---|---|
| Decision ID | To be assigned |
| Decision | Additional QA capacity versus revised release date |
| Decision date | Pending |
| Approver | Steering Committee |
| Conditions | Validate resources, test effort, and recovery |
| Status | Pending |
| Follow-up | Record approval conditions and update delivery plan |

### Management Decisions

1. **Funding:** Determine whether the potential schedule benefit justifies the estimated €12,000 additional cost.
2. **Recovery feasibility:** Confirm whether temporary resources can realistically recover the remaining testing delay.
3. **Release governance:** Preserve mandatory quality criteria regardless of the selected option.
4. **Execution:** Record the decision and activate the approved recovery or revised-release plan.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The paper presents two credible options, consistent cost and schedule comparisons, and a conditional recommendation. However, recovery feasibility and staffing availability are not yet validated.

**Required corrections:** Confirm resource costs, onboarding time, remaining test effort, updated budget forecast, and the impact of either option on release readiness.

**Approval blockers:** Unverified recovery assumptions and incomplete financial and capacity evidence.

**Governance:** Supports PMI-aligned project governance, financial management, schedule recovery, risk assessment, and executive decision-making.

AI can structure and challenge decision papers but cannot authorize expenditure, accept residual risks, or replace Steering Committee approval. Validate financial, technical, contractual, and schedule assumptions before formal submission. Protect confidential commercial, vendor, customer, and project information.
