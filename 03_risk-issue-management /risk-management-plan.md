# Risk Management Plan

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** RISK-006 | **Category:** Risk & Issue Management

---


## 1. Ready-to-Use Prompt

**Purpose:** Establish a consistent, accountable risk-management process to identify, assess, respond to, monitor, and escalate project uncertainty throughout delivery.

**Use case:** Define risk ownership, scoring, mitigation, reporting, and escalation procedures when initiating a software project, establishing delivery governance, or reviewing significant changes to project scope and risk exposure.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager and Risk Management Specialist
experienced in software delivery, technology risk, stakeholder
coordination, uncertainty management, and project governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Project duration: [DURATION]
Target completion: [DATE]
Budget: [BUDGET OR RANGE]
Project team: [ROLES]
External vendors: [IF RELEVANT]
Systems and integrations: [LIST]
Known dependencies: [LIST]
Known constraints: [LIST]
Known risks and issues: [LIST]
Governance structure: [DETAILS]
Risk appetite / tolerance: [APPROVED THRESHOLDS / UNKNOWN]
Existing risk methodology: [DETAILS / NONE]
Reporting requirements: [DETAILS]

TASK

Create a professional Risk Management Plan defining how
project uncertainty will be managed throughout delivery.

1. Define the purpose, scope, and business value of
   the risk-management process.
2. Establish a repeatable process for identifying, assessing,
   prioritizing, responding to, monitoring, and closing risks.
3. Define responsibilities for the Project Manager, Risk Owners,
   Action Owners, Sponsor, technical leads, and governance bodies.
4. Document risk appetite, tolerance thresholds, and approval
   authority where organizational information is available.
5. Establish risk-identification methods and relevant risk domains,
   including technical, business, security, delivery, and vendor risks.
6. Define qualitative scoring using likelihood, impact,
   proximity, dependency exposure, and assessment confidence.
7. Determine when quantitative risk analysis is justified,
   considering schedule, cost, and contingency uncertainty.
8. Define response strategies, mitigation actions,
   contingency triggers, and residual risk assessment.
9. Assign risk ownership based on authority and ability
   to influence outcomes; distinguish Risk and Action Owners.
10. Define monitoring of exposure, mitigation progress,
    early warning indicators, and emerging risks.
11. Establish audience-specific risk reporting and
    management dashboards.
12. Define escalation triggers, recipients, required decisions,
    and authority limits.
13. Specify the minimum fields and controls for the risk register.
14. Establish risk review cadence and event-driven reassessment.
15. Define risk closure criteria, evidence, and treatment
    when a risk materializes into an issue.
16. Establish lessons learned and continuous improvement
    of the risk-management process.

Use organizational standards and approved risk thresholds
where available.

If none are provided, propose a provisional methodology
and flag it for approval.

Separate risks from existing issues.
Distinguish initial exposure from forecast and verified
residual exposure.

Do not invent risk tolerance, ownership, mitigation
effectiveness, financial exposure, or formal approvals.

Adapt controls to the delivery approach without
introducing unnecessary governance layers.

OUTPUT FORMAT

1. PURPOSE AND SCOPE
   Objective | Risk Coverage | Business Value

2. RISK MANAGEMENT APPROACH
   Process Step | Method | Expected Output | Responsible Role

3. ROLES AND RESPONSIBILITIES
   Role | Risk Responsibility | Decision Authority

4. RISK APPETITE AND TOLERANCE
   Risk Dimension | Approved Threshold |
   Escalation Requirement | Authority | Status

5. RISK IDENTIFICATION PROCESS
   Risk Domain | Identification Method |
   Information Source | Review Trigger

6. QUALITATIVE RISK ANALYSIS
   Scoring Model | Rating Thresholds |
   Prioritization Factors | Confidence Requirements

7. QUANTITATIVE RISK ANALYSIS
   Application | Required Inputs | Method |
   Decision Supported | Applicability

8. RISK RESPONSE PLANNING
   Response Strategy | Preventive Action |
   Trigger | Contingency | Residual Risk Review

9. RISK OWNERSHIP
   Risk Category | Proposed Risk Owner |
   Action Owner | Accountability

10. RISK MONITORING
    Monitoring Activity | Indicator |
    Responsible Role | Required Action

11. RISK REPORTING
    Audience | Information Required |
    Format | Frequency | Owner

12. RISK ESCALATION
    Trigger | Recipient | Decision Required |
    Decision Owner | Response Timeframe

13. RISK REGISTER STRUCTURE
    Required Field | Purpose | Update Responsibility

14. RISK REVIEW CADENCE
    Review | Frequency | Participants | Output

15. RISK CLOSURE
    Closure Condition | Evidence Required |
    Approval Authority | Related Issue Action

16. CONTINUOUS IMPROVEMENT
    Review Trigger | Lessons Learned |
    Improvement Action | Owner

MANAGEMENT SUMMARY

- Major risk-management controls
- Unconfirmed risk tolerance and governance arrangements
- Critical ownership and escalation gaps
- Recommended approval decisions
- Immediate implementation actions

Use concise Markdown tables.
Mark unknown information as "Not yet defined".
Label proposed responsibilities and thresholds as unconfirmed.
```

---

## 2. Quality Check

Apply this control after generating the Risk Management Plan.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the Risk Management Plan.

Verify:

1. Completeness: All 16 required components are addressed.
2. Consistency: Risk identification, scoring, responses,
   monitoring, escalation, and closure form one coherent process.
3. Accountability: Risk Owners, Action Owners, and approval
   authorities are clearly differentiated.
4. Evidence: Scoring methods, assumptions, thresholds, and
   residual risk assessments are supported or marked provisional.
5. Governance: Escalation and risk acceptance follow confirmed
   organizational authority.
6. Practicality: Review frequency, reporting, and response
   requirements match project complexity and delivery approach.
7. Integration: Risks, issues, dependencies, and change-control
   procedures are appropriately connected.
8. Actionability: Unresolved governance gaps have specific
   corrective actions and proposed owners.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent risk tolerance, final accountability,
risk acceptance, or mitigation effectiveness.

Flag arrangements requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Software Development — Release Risk Management

**Scenario:** An IT team is developing new reporting functionality for an existing web application. The project depends on backend API development, integration testing, business-user acceptance, and security approval.

The Project Manager must establish a consistent risk-management process before testing and release preparation to prevent late identification of delivery threats.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Phase | Development / Integration |
| Delivery approach | Scrum |
| Target release | 30 June 2027 |
| Team | Project Manager, Product Owner, Developers, QA Lead, Security Lead |
| Systems | Web Application, Reporting API, Database |
| Major dependencies | API readiness, QA capacity, UAT participation, security review |
| Governance | Weekly delivery review, monthly project review |
| Risk tolerance | Not yet defined |
| Management decision | Approve risk responsibilities, review cadence, and escalation procedures before release testing |

### Example Input

```text
Project: Web Application Reporting Enhancement

Business objective:
Deliver new reporting functionality to business users.

Project phase: Development / Integration
Delivery approach: Scrum
Target release: 30 June 2027

Team:
- Project Manager
- Product Owner
- Development Lead
- QA Lead
- Security Lead

Systems:
Web Application
Reporting API
Database

Known dependencies:
- Backend API completion
- Integration testing
- Business-user availability for UAT
- Security approval

Known risks:
R-01: API completion may be delayed.
R-02: Critical defects may remain before release.
R-03: Business users may be unavailable for UAT.
R-04: Security review may identify release blockers.
R-05: Limited QA capacity may delay regression testing.

Governance:
Weekly delivery review
Monthly project review

Risk appetite and tolerance:
Not yet formally defined.

Reporting:
Weekly project status report.
Material risks escalated to project leadership.

Management objective:
Define a repeatable risk-management process
and assign clear responsibilities before release testing.
```

### Example Output — Risk Management Plan

#### 1. Purpose and Scope

| Objective | Risk Coverage | Business Value |
|---|---|---|
| Identify delivery threats early | Development, integration, testing | Reduced delivery uncertainty |
| Establish accountability | Risk responses and decisions | Faster resolution |
| Protect release readiness | Quality, security, business acceptance | Informed release decisions |

#### 2. Risk Management Approach

| Step | Method | Expected Output | Proposed Owner |
|---|---|---|---|
| Identify | Team and dependency reviews | New risk candidates | Project Manager / Leads |
| Assess | Qualitative scoring | Prioritized risks | Risk Owners |
| Plan response | Mitigation and contingency | Action plan | Risk Owners |
| Monitor | Weekly risk review | Updated register | Project Manager |
| Escalate | Defined triggers and authority | Management decision | Project Manager |
| Close | Verified closure criteria | Closure record | Risk Owner |

#### 3. Roles and Responsibilities

| Role | Risk Responsibility | Decision Authority |
|---|---|---|
| Project Manager | Coordinate risk process and reporting | Within approved delegation |
| Product Owner | Assess product and business risks | Product decisions within authority |
| Development Lead | Assess technical and integration risks | Technical decisions within authority |
| QA Lead | Assess testing and quality risks | Testing decisions within authority |
| Security Lead | Assess security exposure | Per security governance |
| Project Sponsor | Review escalated material exposure | Subject to formal delegation |

All responsibility and authority assignments require confirmation.

#### 4. Risk Appetite and Tolerance

| Dimension | Approved Threshold | Escalation Requirement | Authority | Status |
|---|---|---|---|---|
| Schedule | Not defined | Material release threat | TBD | Pending |
| Cost | Not defined | Exceeds delegated budget authority | TBD | Pending |
| Quality | Not defined | Release acceptance threatened | TBD | Pending |
| Security | Not defined | Material security exposure | Security authority TBD | Pending |

**Management requirement:** Confirm organizational tolerance and approval authority before formal risk acceptance.

#### 5. Risk Identification Process

| Domain | Method | Information Source | Review Trigger |
|---|---|---|---|
| Integration | Dependency review | API delivery status | Integration milestone |
| Quality | Defect trend review | Jira / test results | Testing review |
| Resources | Capacity review | Team availability | Capacity change |
| Business | UAT readiness review | Business commitments | UAT planning |
| Security | Security assessment | Security findings | Security review |

#### 6. Qualitative Risk Analysis

A provisional 5×5 model is proposed, subject to governance approval.

**Risk score = Likelihood × Impact**

| Score | Rating | Proposed Management Approach |
|---|---|---|
| 1–4 | Low | Periodic review |
| 5–9 | Medium | Monitor and manage |
| 10–16 | High | Active mitigation |
| 17–25 | Critical | Urgent management review |

Likelihood and impact use scales from 1 to 5.

Prioritization must also consider risk proximity, shared dependencies, recovery difficulty, business consequences, and confidence in the assessment.

Risk scoring is performed separately using the approved method; no project-specific scores are inferred from the current input.

#### 7. Quantitative Risk Analysis

| Application | Required Inputs | Method | Decision Supported | Applicability |
|---|---|---|---|---|
| Release delay exposure | Activity dependencies, durations, uncertainty | Schedule scenario analysis | Release feasibility | Assess if material |
| Additional testing capacity | Resource rates, effort forecasts | Cost scenario analysis | Resource allocation | Assess if required |
| Budget contingency | Estimated financial exposure | Contingency analysis | Funding decision | Insufficient inputs |

Quantitative analysis should be performed only when reliable input data can support meaningful conclusions.

#### 8. Risk Response Planning

| Risk | Proposed Strategy | Preventive Action | Trigger / Contingency | Residual Review |
|---|---|---|---|---|
| R-01 API delay | Mitigate | Confirm delivery forecast and integration checkpoints | Activate approved recovery approach if SIT is threatened | After API readiness evidence |
| R-02 Critical defects | Mitigate | Review defect trends and testing coverage | Escalate if release criteria are threatened | After verified fixes |
| R-03 UAT availability | Mitigate | Confirm business-user commitments | Escalate capacity gap before UAT | After allocation confirmed |
| R-04 Security blockers | Mitigate | Review security requirements early | Escalate material findings | After security assessment |
| R-05 QA capacity | Mitigate | Validate regression workload and staffing | Review approved capacity options | After capacity validation |

Planned mitigation does not automatically reduce residual risk.

#### 9. Risk Ownership and Allocation

| Risk Category | Proposed Risk Owner | Proposed Action Owner | Accountability |
|---|---|---|---|
| Integration | Development Lead | Backend Developer | API readiness |
| Testing / Quality | QA Lead | QA / Development Team | Defect and test exposure |
| UAT / Business | Product Owner | Business Representative | UAT availability |
| Security | Security Lead | Assigned Security Specialist | Security assessment |
| Resource Capacity | Project Manager | QA Lead | Capacity coordination |

Each material risk requires one confirmed Risk Owner, even where multiple individuals execute mitigation actions.

#### 10. Risk Monitoring

| Activity | Indicator | Proposed Owner | Required Action |
|---|---|---|---|
| Integration monitoring | API readiness / missed checkpoints | Development Lead | Reassess schedule exposure |
| Defect monitoring | Open critical defects and trends | QA Lead | Update risk response |
| UAT readiness | Confirmed business-user availability | Product Owner | Resolve capacity gaps |
| Security review | Open approval findings | Security Lead | Review release exposure |
| Mitigation tracking | Overdue response actions | Project Manager | Escalate where necessary |

#### 11. Risk Reporting

| Audience | Information Required | Format | Frequency | Proposed Owner |
|---|---|---|---|---|
| Delivery Team | Active risks, actions, dependencies | Team review / Jira | Weekly (proposed) | Project Manager |
| Project Leadership | High and Critical risks, mitigation progress | Risk summary | Weekly (proposed) | Project Manager |
| Project Sponsor | Material exposure and decisions | Management report | Monthly (existing review) | Project Manager |
| Security Authority | Material security risks | Security assessment | Event-driven | Security Lead |

The proposed dashboard should show active risks, High/Critical exposure, overdue mitigation, emerging risks, and escalation decisions.

#### 12. Risk Escalation

| Trigger | Proposed Recipient | Decision Required | Decision Owner | Response Timeframe |
|---|---|---|---|---|
| Release milestone threatened | Project Sponsor | Recovery or commitment change | TBD | TBD |
| Mitigation requires additional funding | Authorized budget approver | Resource / funding decision | TBD | TBD |
| Material security exposure | Security authority | Security risk treatment | TBD | Per policy |
| Risk exceeds tolerance | Appropriate governance body | Risk response or acceptance | TBD | TBD |

Escalation should occur when a material threshold is reached, not only during scheduled reporting.

#### 13. Risk Register Structure

| Required Field | Purpose | Update Responsibility |
|---|---|---|
| Risk ID / Category | Identification and classification | Project Manager |
| Risk statement / Cause / Impact | Define uncertainty and consequences | Risk Owner |
| Likelihood / Impact / Rating | Assess exposure | Risk Owner |
| Proximity / Warning indicator | Track urgency | Risk Owner |
| Response / Contingency | Plan treatment | Risk Owner |
| Action Owner / Due Date | Track implementation | Action Owner |
| Residual Rating / Evidence | Validate remaining exposure | Risk Owner |
| Review Date / Status | Maintain current risk information | Project Manager |

#### 14. Risk Review Cadence

| Review | Frequency | Participants | Output |
|---|---|---|---|
| Delivery risk review | Weekly (proposed) | PM, Technical Leads, QA | Updated risk register |
| Release risk assessment | Before release milestones | Delivery, QA, Security, Product Owner | Release risk assessment |
| Project governance review | Monthly (existing review) | Sponsor / Project Leadership | Decisions and escalations |
| Event-driven reassessment | After material changes | Relevant Risk Owners | Updated exposure and actions |

#### 15. Risk Closure

| Closure Condition | Required Evidence | Proposed Approval Authority | Related Issue Action |
|---|---|---|---|
| Risk can no longer occur | Verified condition | Risk Owner / governance TBD | None required |
| Exposure period has passed | Milestone and risk review | Risk Owner | None required |
| Dependency resolved | Completion evidence | Risk Owner | Close related actions |
| Risk materialized | Confirmed event | Risk Owner / PM | Link to active issue |
| Residual exposure accepted | Authorized acceptance record | Approved risk authority | Track residual obligations |

Risk acceptance does not automatically mean the underlying exposure has disappeared. Accepted exposure should remain visible and monitored where required by the organization's governance rules.

#### 16. Continuous Improvement

| Review Trigger | Lessons Learned | Improvement Action | Proposed Owner |
|---|---|---|---|
| Significant risk materializes | Identify missed warning indicators | Improve identification and monitoring | Project Manager |
| Release milestone completed | Evaluate response effectiveness | Update risk practices | Risk Owners |
| Repeated dependency failures | Identify systemic ownership gaps | Improve dependency governance | Project Manager |
| Project closure | Review risk outcomes | Document reusable lessons | Project Manager / PMO |

### Management Decisions

1. **Risk governance:** Approve the scoring model, organizational tolerance thresholds, and escalation authority.
2. **Accountability:** Confirm individual Risk Owners and Action Owners across integration, testing, business, and security.
3. **Response planning:** Establish actionable mitigation and contingency plans for risks threatening SIT, UAT, or release readiness.
4. **Monitoring and reporting:** Confirm the review cadence, risk register ownership, and escalation procedures before formal release planning.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The proposed plan covers all 16 management components and defines a coherent risk lifecycle. However, organizational risk tolerance, final ownership, escalation response timeframes, and formal risk acceptance authority remain unconfirmed.

**Required corrections:**
- Validate the qualitative scoring methodology.
- Define and approve risk tolerance thresholds.
- Confirm risk ownership and escalation responsibilities.
- Agree on mitigation monitoring and reporting expectations.
- Establish formal residual risk acceptance and closure procedures.

**Approval blockers:** Undefined risk tolerance, unconfirmed risk acceptance authority, and incomplete governance responsibilities.

**Governance:** This prompt supports relevant PMI-aligned risk management practices and ISO 31000-style principles of structured, integrated, and continuously reviewed risk management.

The Risk Management Plan defines how risks will be managed; it does not replace the project risk register, approved governance procedures, or accountable human judgment. Formal risk acceptance and security-related decisions remain with authorized stakeholders. Protect confidential technical, commercial, customer, financial, and security-sensitive information.
