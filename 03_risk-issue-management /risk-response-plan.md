# Risk Response Plan

**Prompt ID:** RISK-004 | **Category:** Risk & Issue Management | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Convert prioritized project risks into specific, owned, time-bound actions that reduce exposure and establish clear contingency and escalation procedures.

**Use case:** Develop risk responses when software integrations, testing, resources, vendors, or release dependencies threaten agreed IT project objectives.

Copy the prompt and replace the placeholders with your project information.

```text id="n8f2aa"
ROLE

You are a Senior IT Project Manager and Risk Management Specialist
experienced in software delivery, technical dependencies,
risk response planning, vendor coordination, and governance.

CONTEXT

Project: [PROJECT NAME]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target milestone: [DATE / MILESTONE]
Prioritized risks: [PASTE RISK REGISTER]
Current risk ratings: [VALUES]
Risk tolerance: [APPROVED THRESHOLDS / UNKNOWN]
Existing mitigation: [ACTIONS / NONE]
Known constraints: [LIST]
Available resources: [ROLES / CAPACITY]
Approval authority: [ROLES / UNKNOWN]
Review date: [DATE]

TASK

Create an actionable Risk Response Plan for the priority risks.

STEP 1 — RESPONSE STRATEGY

1. Select and justify an appropriate response:
   - Avoid: Eliminate the threat by changing the approach.
   - Mitigate: Reduce likelihood and/or impact.
   - Transfer / Share: Allocate part of the exposure
     through a suitable agreement or arrangement.
   - Accept: Retain exposure within authorized tolerance.
   - Escalate: Refer decisions beyond project authority.

2. Assess response feasibility, dependencies, resource
   requirements, costs, and delivery-model implications.

STEP 2 — PREVENTIVE ACTIONS AND CONTINGENCY

3. Define specific preventive actions with:
   - Action and intended result
   - Risk Owner and Action Owner
   - Deadline
   - Expected risk reduction
   - Evidence of completion

4. Identify measurable early warning indicators
   and contingency activation triggers.
5. Define contingency actions if the risk materializes.
6. Identify interconnected risks requiring coordinated responses.

STEP 3 — RESIDUAL EXPOSURE AND ESCALATION

7. Compare initial and expected residual likelihood,
   impact, score, and rating.
8. Distinguish forecast residual exposure from verified
   exposure after mitigation has been implemented.
9. Identify escalation triggers, decision authority,
   and approval requirements.
10. Define monitoring, response-effectiveness checks,
    and review dates.

Avoid generic actions such as "monitor closely"
or "follow up regularly" without measurable outputs.

Do not invent deadlines, approved thresholds, resources,
contractual commitments, or mitigation effectiveness.

Do not mark risk acceptance as approved unless
authorization is explicitly provided.

OUTPUT FORMAT

1. RISK RESPONSE PLAN

Risk ID | Current Rating | Strategy | Rationale |
Preventive Action | Trigger | Contingency |
Risk Owner | Action Owner | Deadline | Review Date

2. ACTION TRACKER

Action | Expected Risk Reduction | Owner |
Due Date | Completion Evidence | Status

3. DEPENDENCY-BASED RESPONSES

Related Risks | Common Dependency | Coordinated Action |
Coordination Owner | Escalation Trigger

4. RESIDUAL RISK ASSESSMENT

Risk ID | Initial L / I / Score / Rating |
Mitigation Status | Forecast Residual L / I / Score / Rating |
Verified Residual Exposure | Evidence |
Acceptable Against Approved Tolerance?

5. ESCALATION AND DECISIONS

Risk ID | Escalation Trigger | Decision Required |
Decision Owner | Decision Deadline | Impact if Delayed

6. MANAGEMENT SUMMARY

- Highest-priority response actions
- Critical dependencies and contingencies
- Residual exposure and evidence gaps
- Decisions requiring authorization
- Immediate management priorities

Use concise Markdown tables.
Mark missing information as "Not yet defined".
Clearly label unapproved actions and forecast residual scores.
```

---

## 2. Quality Check

Apply this independent review after generating the Risk Response Plan.

```text id="q6fr11"
QUALITY CHECK

Act as a Senior QA Manager reviewing the Risk Response Plan.

Verify:

1. Coverage: Each priority risk has an appropriate response strategy.
2. Actionability: Actions specify owners, deadlines,
   measurable outcomes, and completion evidence.
3. Prevention: Preventive actions, triggers, and
   contingency responses are clearly distinguished.
4. Feasibility: Cost, capacity, technical dependencies,
   and delivery constraints are considered.
5. Residual Risk: Score reductions are justified;
   forecast and verified exposure are separated.
6. Governance: Escalation, risk acceptance,
   and funding decisions follow approved authority.
7. Monitoring: Response effectiveness can be verified
   and unsuccessful responses can be revised.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Identify vague actions and replace them with specific,
measurable recommendations.
Do not invent approval, capacity, or effectiveness evidence.
```

---

## 3. Practical IT Use Case

### Software Development — Third-Party API Capacity Risk

**Scenario:** An IT team is implementing automated customer notifications using an external email API. Initial development is progressing, but expected notification volume may exceed the provider's current API rate limit during peak periods.

The Project Manager must establish preventive controls, contingency options, and escalation procedures before production release.

### Project Context

| Attribute | Details |
|---|---|
| Project | Customer Notification Automation |
| Phase | Development / Integration Testing |
| Delivery approach | Scrum |
| Target release | 30 September 2027 |
| Systems | Web Application, Notification Service, Email API |
| External dependency | Third-party Email Provider |
| Key risk | API capacity may be insufficient during peak demand |
| Management decision | Approve a capacity-validation and fallback approach before go-live |

### Example Input

```text id="k2rsa4"
Project: Customer Notification Automation

Business objective:
Automate customer email notifications for application events.

Phase: Development / Integration Testing
Delivery approach: Scrum
Target release: 30 September 2027

Risk ID: R-03
Risk statement:
If peak notification volume exceeds the email provider's
rate limit, messages may be delayed or rejected,
affecting customer communication.

Current likelihood: 4 — Likely
Current impact: 4 — Major
Current score: 16 — High

Known information:
- Current provider limit: 100 requests/minute.
- Peak demand forecast: 180 requests/minute.
- Load testing has not yet been completed.
- Message queuing is technically possible.
- Higher provider capacity may require additional cost.

Risk Owner: Technical Lead
Action Owners: Backend Developer / QA Lead

Risk tolerance: Not formally defined.
Target mitigation deadline: Not yet agreed.
Approval authority: Not yet confirmed.
```

### Example Output — Risk Response Plan

#### 1. Risk Response Plan

| Field | Proposed Response |
|---|---|
| Risk ID | R-03 |
| Current exposure | 4 × 4 = 16 — High |
| Response strategy | Mitigate |
| Rationale | Reduce the likelihood of delayed or rejected messages before release |
| Preventive action | Validate API capacity, implement controlled queuing and retry behavior, and perform load testing |
| Early warning | Request volume approaching the approved operating threshold |
| Contingency | Activate an approved rate-limiting or capacity-expansion approach |
| Risk Owner | Technical Lead |
| Action Owners | Backend Developer / QA Lead |
| Deadline | TBD — before release readiness |
| Review date | TBD |

The current forecast exceeds the stated provider limit by 80 requests per minute. The team must validate actual usage patterns, provider enforcement, and queueing behavior before deciding on the final technical response.

#### 2. Action Tracker

| Action | Expected Risk Reduction | Proposed Owner | Due Date | Completion Evidence |
|---|---|---|---|---|
| Validate provider limits | Reduce capacity uncertainty | Technical Lead | TBD | Confirmed provider limits |
| Implement queueing and retry controls | Reduce message rejection and loss | Backend Developer | TBD | Technical test evidence |
| Perform peak-load testing | Validate processing behavior | QA Lead | TBD | Approved load-test results |
| Evaluate higher API capacity | Establish fallback feasibility | Project Manager / Vendor Lead | TBD | Commercial and technical assessment |
| Define alert thresholds | Enable early detection | Technical Lead | TBD | Monitoring configuration evidence |

Implementation remains subject to technical review and approval.

#### 3. Dependency-Based Responses

| Related Risks | Common Dependency | Coordinated Action | Proposed Owner | Escalation Trigger |
|---|---|---|---|---|
| API capacity / Message delays | Provider request limits | Coordinate queuing and capacity validation | Technical Lead | Load tests fail agreed criteria |
| API capacity / Release readiness | Third-party API | Confirm acceptable throughput before release | Project Manager | Release acceptance at risk |
| Provider capacity / Cost | Commercial API plan | Review upgrade cost and authority | Project Manager | Additional funding required |

#### 4. Residual Risk Assessment

| Measure | Assessment |
|---|---|
| Initial likelihood | 4 |
| Initial impact | 4 |
| Initial score / rating | 16 — High |
| Mitigation status | Proposed |
| Forecast residual likelihood | Not assessed |
| Forecast residual impact | Not assessed |
| Verified residual exposure | Not assessed |
| Effectiveness evidence | Load testing and monitoring results required |
| Residual exposure acceptable? | Undetermined — tolerance not defined |

**Management interpretation:** Queuing and retry controls may reduce message loss, but they do not necessarily eliminate delivery delays. Residual risk must be evaluated against agreed delivery-time and reliability requirements.

#### 5. Escalation and Decisions

| Trigger | Decision Required | Proposed Decision Owner | Deadline |
|---|---|---|---|
| Load tests fail acceptance criteria | Approve technical recovery approach | Technical Lead / authorized authority | Before release approval |
| Additional provider capacity required | Approve commercial change | Budget approver TBD | Before procurement commitment |
| Required notification performance cannot be met | Reassess release readiness | Authorized release approver TBD | Before go-live |

### Management Decisions

1. **Technical mitigation:** Confirm whether queuing, retry handling, and provider capacity are sufficient for expected demand.
2. **Quality assurance:** Approve measurable load-test acceptance criteria and monitoring thresholds.
3. **Commercial contingency:** Evaluate a higher-capacity API plan and identify the authorized budget approver.
4. **Release governance:** Require evidence of acceptable notification performance before approving production deployment.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The response strategy addresses the known API limitation and defines actionable mitigation and contingency options. However, load-test acceptance criteria, action deadlines, commercial approval, and verified residual risk remain unresolved.

**Required corrections:**
- Confirm expected peak volume and provider limits.
- Define measurable delivery-performance thresholds.
- Assign and approve mitigation deadlines.
- Validate queueing and retry behavior through testing.
- Establish contingency and release approval authority.
- Reassess residual exposure using test evidence.

**Approval blockers:** Unverified performance capacity, undefined risk tolerance, and unconfirmed funding and release authority.

**Governance:** Supports PMI-aligned risk response planning, ownership, contingency management, monitoring, and escalation.

Risk responses and residual risk acceptance require validation by accountable technical, business, and governance stakeholders. Do not expose confidential architecture, vendor contracts, security information, or customer data in public AI tools.
