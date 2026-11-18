# Schedule Narrative

**Prompt ID:** PLAN-002 | **Category:** Project Planning | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Translate project schedule data into a clear management narrative explaining delivery logic, milestone dependencies, schedule risks, and required decisions.

**Use case:** Prepare schedule commentary for weekly project status reports, steering committee reviews, release planning, or recovery discussions when milestones or dependencies are at risk.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software delivery,
schedule management, dependency analysis, delivery forecasting,
risk management, and executive reporting.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Planned start: [DATE]
Target completion: [DATE]
Major phases / workstreams: [LIST]
Milestones and planned dates: [LIST]
Actual / forecast milestone dates: [IF AVAILABLE]
Internal dependencies: [LIST]
External dependencies: [LIST]
Schedule constraints: [LIST]
Current schedule status: [ON TRACK / AT RISK / DELAYED / UNKNOWN]
Known variances: [DETAILS]
Recovery actions: [IF AVAILABLE]
Schedule baseline: [APPROVED / DRAFT / NOT DEFINED]

TASK

Create a professional Schedule Narrative from the available information.

1. Summarize the overall timeline, delivery status, and target completion.
2. Explain major phases, workstreams, and milestone sequencing.
3. Identify dependencies influencing milestone achievement.
4. Explain parallel activities, handoffs, and coordination requirements.
5. Identify the critical path only where sufficient schedule
   logic and duration data are available; otherwise flag
   potentially critical dependencies.
6. Assess milestone variances against the available baseline.
7. Identify schedule risks, causes, impacts, and early warning indicators.
8. Assess constraints, external dependencies, and approval lead times.
9. Evaluate recovery options, including re-sequencing,
   parallel delivery, resource adjustments, or scope changes.
10. Identify risks, trade-offs, and approval requirements
    associated with proposed recovery actions.
11. Classify schedule health as GREEN, AMBER, or RED,
    supported by available evidence.
12. Recommend management actions and decisions required
    to protect or revise the delivery commitments.

Explain why dates and dependencies matter.
Do not simply repeat a milestone list.
Do not invent dates, durations, schedule float, or recovery capacity.
Distinguish confirmed plans from forecasts and assumptions.
Adapt the narrative to the stated delivery approach.

OUTPUT FORMAT

1. SCHEDULE NARRATIVE
   Write concise management commentary covering:
   - Overall timeline and delivery status
   - Major phases and milestones
   - Sequencing and parallel work
   - Critical dependencies
   - Current variances and risks
   - Recovery approach and required decisions

2. MILESTONE STATUS
   Milestone | Baseline Date | Forecast Date |
   Variance | Status | Owner

3. CRITICAL DEPENDENCIES
   Dependency | Required By | Owner |
   Current Status | Impact if Late

4. SCHEDULE RISKS
   Risk | Cause | Potential Impact |
   Early Warning Indicator | Mitigation | Owner

5. SCHEDULE HEALTH
   GREEN: Major milestones achievable under the current plan.
   AMBER: Delivery remains potentially achievable but requires
          active mitigation or resolution of material dependencies.
   RED: Current commitments are not achievable without
        significant intervention or formal change.

   Provide Status | Rationale | Confidence.

   If evidence is insufficient, report "Not assessable"
   rather than assigning an unsupported health status.

6. RECOVERY OPTIONS
   Option | Expected Benefit | Risk / Trade-Off |
   Decision Owner | Recommendation

7. MANAGEMENT DECISIONS
   Decision Required | Priority | Proposed Owner |
   Required By | Expected Outcome

Use concise Markdown tables.
Mark missing information as "Not yet defined".
Label unapproved recovery actions and revised dates as proposed.
```

---

## 2. Quality Check

Apply this control after generating the Schedule Narrative.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the Schedule Narrative.

Verify:

1. Accuracy: Dates, milestone sequences, and variances are consistent
   with the provided schedule data.
2. Completeness: Major milestones, dependencies, risks,
   recovery options, and management decisions are covered.
3. Schedule Logic: Dependencies, parallel activities, and
   potentially critical delivery paths are explained correctly.
4. Evidence: Baselines, forecasts, schedule health, and
   critical-path claims are supported by available information.
5. Risk: Material schedule threats and early warning indicators
   are identified.
6. Feasibility: Recovery recommendations consider capacity,
   quality, cost, dependencies, and approval requirements.
7. Governance: Re-baselining, scope changes, and delivery
   commitments are subject to appropriate authorization.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [UNRESOLVED CRITICAL ITEMS]

Do not invent dates, float, dependencies, or recovery capacity.
Flag schedule conclusions requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Software Development — API Integration Delay Before Release

**Scenario:** A software team is developing new reporting functionality for a web application. Frontend development is progressing as planned, but an API integration delay is threatening the start of system integration testing (SIT).

The Project Manager must explain the schedule implications to stakeholders and recommend recovery actions before the planned release.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Phase | Development / Integration |
| Delivery approach | Scrum with release milestones |
| Planned start | 1 March 2027 |
| Target release | 30 June 2027 |
| Current reporting date | 10 May 2027 |
| Team | 4 Developers, 2 QA Engineers, 1 Product Owner, 1 Project Manager |
| Critical dependency | Backend reporting API |
| Known issue | API completion forecast two weeks later than planned |
| Management decision | Determine whether the release date remains achievable and identify recovery actions |

### Example Input

```text
Project: Web Application Reporting Enhancement

Business objective:
Deliver enhanced reporting functionality to business users.

Delivery approach: Scrum
Planned start: 1 March 2027
Target release: 30 June 2027
Reporting date: 10 May 2027

Milestones:
Requirements approval — 15 March (completed)
Frontend development — 30 April (completed)
Backend API completion — 15 May (forecast 29 May)
System Integration Testing — 16 May to 5 June
User Acceptance Testing — 8 June to 19 June
Release readiness approval — 25 June
Production release — 30 June

Dependencies:
- Frontend integration requires the reporting API.
- SIT requires integrated functionality.
- UAT requires completion of relevant integration tests.
- Production release requires UAT and release readiness approval.

Known schedule risk:
Backend API completion is forecast two weeks late.

Constraints:
- QA team has limited availability.
- Release target is linked to a business reporting cycle.
- Additional development capacity is not confirmed.

Current status:
At risk.

Recovery options under consideration:
- Prioritize critical API endpoints.
- Prepare integration tests using mocks.
- Review opportunities for parallel testing.
- Defer non-critical reporting features, subject to approval.
```

### Example Output — Schedule Narrative

#### 1. Schedule Narrative

The Web Application Reporting Enhancement project is scheduled for delivery between **1 March and 30 June 2027**, with the production release aligned to the business reporting cycle.

Requirements approval and frontend development are complete. However, backend API completion is now forecast for **29 May**, compared with the planned date of **15 May**, creating a 14-calendar-day variance.

System Integration Testing was scheduled to begin on 16 May. Because integrated functionality depends on the reporting API, the forecast delay threatens the original testing window.

Preparation of test data, integration test cases, and mock-based testing may proceed in parallel, subject to technical feasibility. However, these activities cannot fully replace testing against the completed production-intended API.

UAT is planned for 8–19 June, followed by release readiness approval on 25 June. The available schedule leaves limited time to absorb additional integration or testing delays.

**Schedule assessment:** AMBER — the June release may remain achievable, but only if the integration impact is contained and an evidence-based recovery plan is agreed.

The immediate priority is to validate API readiness, reassess the testing sequence, and confirm whether critical functionality can be completed without compromising release quality.

#### 2. Milestone Status

| Milestone | Baseline Date | Forecast Date | Variance | Status | Proposed Owner |
|---|---|---|---|---|---|
| Requirements approval | 15 Mar | 15 Mar | 0 days | Complete | Product Owner |
| Frontend development | 30 Apr | 30 Apr | 0 days | Complete | Development Lead |
| Backend API completion | 15 May | 29 May | +14 calendar days | Delayed forecast | Backend Lead |
| SIT completion | 5 Jun | TBD | Not assessable | At risk | QA Lead |
| UAT completion | 19 Jun | TBD | Not assessable | At risk | Product Owner |
| Release readiness approval | 25 Jun | TBD | Not assessable | At risk | Authorized approver TBD |
| Production release | 30 Jun | TBD | Not assessable | At risk | Release authority TBD |

*The milestone dates are supplied planning dates; formal baseline approval and proposed ownership require confirmation.*

#### 3. Critical Dependencies

| Dependency | Required By | Proposed Owner | Current Status | Impact if Late |
|---|---|---|---|---|
| Backend reporting API | SIT start | Backend Lead | Forecast delayed | Integrated testing cannot begin as planned |
| API integration | SIT completion | Development Lead | At risk | Testing window may be compressed |
| SIT completion | UAT start | QA Lead | At risk | UAT start may be delayed |
| Business-user availability | UAT period | Product Owner | Not confirmed | UAT completion may slip |
| Release readiness approval | 25 Jun | TBD | Pending | Production release cannot proceed without approval |

The backend API is a potentially critical schedule dependency. A formal critical-path assessment requires validated activity relationships, durations, and available float.

#### 4. Schedule Risks

| Risk | Cause | Potential Impact | Early Warning Indicator | Mitigation | Proposed Owner |
|---|---|---|---|---|---|
| API delivery delay | Backend development behind plan | SIT delay | Critical endpoints incomplete | Prioritize API functionality | Backend Lead |
| Compressed testing | Reduced available SIT window | Undetected defects | Falling test completion rate | Re-sequence eligible tests | QA Lead |
| UAT delay | Late SIT completion | Release approval delay | UAT entry criteria not met | Confirm UAT readiness plan | Product Owner |
| Resource constraint | Limited QA capacity | Testing backlog | Growing unexecuted test cases | Review capacity and priorities | Project Manager |
| Release quality risk | Accelerated delivery | Production defects | Unresolved critical defects | Maintain release quality gates | QA Lead |

#### 5. Schedule Health

| Assessment | Result |
|---|---|
| Schedule status | AMBER |
| Primary concern | API completion forecast 14 calendar days late |
| Milestone exposure | SIT, UAT, release readiness |
| Recovery feasibility | Not yet validated |
| Assessment confidence | Limited — downstream forecasts and float unavailable |

**Rationale:** The release target has not yet been demonstrated to be unachievable, but the known integration delay threatens the testing sequence and requires immediate mitigation.

#### 6. Recovery Options

| Option | Potential Benefit | Risk / Trade-Off | Proposed Decision Owner | Recommendation |
|---|---|---|---|---|
| Prioritize critical API endpoints | Enables earlier integration of essential functionality | Remaining functionality may be delayed | Product Owner / Development Lead | Assess feasibility |
| Prepare tests using mocks | Reduces testing preparation time | Does not replace real integration validation | QA Lead | Proceed where appropriate |
| Parallelize eligible testing | Reduces sequential waiting | Requires coordination and sufficient QA capacity | QA Lead | Validate capacity |
| Add temporary development capacity | May improve delivery throughput | Onboarding overhead and additional cost | Project Sponsor | Assess only if justified |
| Defer non-critical features | Protects essential release scope | Reduces delivered functionality | Product Owner / Authorized Approver | Consider through scope governance |

Recovery actions must not bypass mandatory testing, security review, or release approval.

#### 7. Management Decisions

| Decision Required | Priority | Proposed Owner | Required By | Expected Outcome |
|---|---|---|---|---|
| Confirm API delivery forecast | High | Backend Lead | Immediately | Reliable integration date |
| Reassess SIT and UAT sequencing | High | QA Lead / Project Manager | Before revised test planning | Updated delivery forecast |
| Validate testing capacity | High | Project Manager | Before recovery commitment | Feasible recovery plan |
| Review potential scope deferral | High | Product Owner | Before release scope decision | Agreed essential functionality |
| Confirm release feasibility | High | Authorized Release Authority | Before release readiness approval | Evidence-based go/no-go decision |

### Management Decisions

1. **Integration priority:** Confirm the API completion forecast and whether critical endpoints can be delivered earlier.
2. **Testing feasibility:** Validate the revised SIT and UAT schedule without reducing mandatory quality controls.
3. **Recovery approach:** Select feasible mitigation measures based on capacity, cost, and delivery risk.
4. **Release governance:** Confirm whether the 30 June release remains achievable or requires a formally approved change.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The narrative identifies the API delay and its likely downstream effects. However, the recovery feasibility, revised testing dates, activity float, and release approval authority remain unconfirmed.

**Required corrections:**
- Validate the revised API completion estimate.
- Recalculate SIT and UAT forecasts using actual dependencies and capacity.
- Confirm business-user and QA availability.
- Assess recovery options against quality and cost constraints.
- Confirm release decision authority and any change-control requirements.

**Approval blockers:** Unvalidated recovery schedule, incomplete downstream milestone forecasts, and unconfirmed release authority.

**Governance:** This prompt supports relevant PMI-aligned practices in schedule planning, milestone control, dependency management, forecasting, risk management, and project governance.

The Schedule Narrative is a management reporting artifact, not a replacement for the approved project schedule. Delivery forecasts, recovery actions, and changed commitments require validation by the Project Manager, Delivery Lead, QA Lead, and relevant governance authorities. Protect confidential project, contractual, financial, and security-sensitive information.
