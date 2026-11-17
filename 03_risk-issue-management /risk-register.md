# Project Risk Register

## Purpose

Use this prompt to create or review a structured project risk register for an IT, software, digital transformation, data, infrastructure, or technology-enabled project.

The register should help the Project Manager:

- identify uncertainty,
- assess exposure,
- prioritise management attention,
- define responses,
- assign ownership,
- establish early warning indicators,
- and monitor risk over time.

The objective is not to produce the longest possible risk list.

The objective is to identify the risks that could materially affect project outcomes and make them manageable.

---

## Best Used For

**Project phase:**  
Initiation / Planning / Delivery / Testing / Deployment

**Project type:**  
Software implementation / Digital transformation / Data / Infrastructure / ERP / Cloud / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / PMO / Risk Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At initiation and reviewed regularly throughout delivery

---

# Prompt

```text id="risk-01"
ROLE

You are a senior IT Project Manager and risk-management specialist
experienced in international software delivery, digital transformation,
third-party dependencies, project governance, and technology risk.

TASK

Create a professional project risk register for the project described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[OBJECTIVE]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Target completion:
[DATE]

Budget:
[BUDGET OR RANGE]

Team structure:
[DETAILS]

Key stakeholders:
[LIST]

External vendors:
[LIST]

Systems involved:
[LIST]

Known dependencies:
[LIST]

Known constraints:
[LIST]

Known assumptions:
[LIST]

Known risk areas:
[LIST]

OUTPUT FORMAT

Create a risk register with:

Risk ID
Risk Category
Risk Statement
Cause
Potential Event
Potential Impact
Likelihood (1-5)
Impact (1-5)
Risk Score
Risk Rating
Early Warning Indicator
Mitigation / Preventive Action
Contingency / Response Action
Risk Owner
Action Owner
Review Date
Status
```

---

# Risk Statement Structure

Write risks using a clear cause-event-impact structure.

Preferred format:

```text id="risk-cause-event-impact"
Because of [CAUSE],
there is a risk that [UNCERTAIN EVENT],
which may result in [PROJECT IMPACT].
```

### Weak

```text id="risk-weak"
Vendor delay.
```

### Better

```text id="risk-better"
Because the external identity provider has limited implementation
capacity, there is a risk that API certification will not complete
before the planned integration-test window, which may delay SIT
and the downstream release schedule.
```

This makes the risk easier to analyse and manage.

---

# Risk Categories

Use categories appropriate to the project.

Possible categories include:

```text id="risk-categories"
Schedule
Scope
Budget
Resources
Technology
Architecture
Integration
Data
Security
Quality
Testing
Vendor
Procurement
Compliance
Operations
Stakeholder
Governance
Change
Business Readiness
External
```

Do not force every project to contain risks in every category.

---

# Risk Scoring

Use a simple 1–5 scale unless the organisation already has an approved risk methodology.

## Likelihood

```text id="risk-likelihood"
1 = Rare
2 = Unlikely
3 = Possible
4 = Likely
5 = Very Likely
```

## Impact

```text id="risk-impact"
1 = Minimal
2 = Minor
3 = Moderate
4 = Major
5 = Severe
```

## Risk Score

```text id="risk-score"
Risk Score = Likelihood × Impact
```

Example classification:

```text id="risk-rating"
1–4   = Low
5–9   = Medium
10–16 = High
17–25 = Critical
```

Use the organisation's approved thresholds if they differ.

---

# Impact Assessment

Where relevant, assess impact across more than one dimension.

Possible dimensions:

```text id="risk-impact-dimensions"
Schedule
Budget
Scope
Quality
Security
Compliance
Operations
Customer
Reputation
Business Value
```

A risk may be moderate financially but critical from a security or regulatory perspective.

---

# Early Warning Indicators

Each significant risk should have an observable indicator.

Examples:

| Risk | Early Warning Indicator |
|---|---|
| Vendor delay | Milestones repeatedly missed |
| UAT delay | Business tester availability below plan |
| Integration risk | API defects remain unresolved near SIT |
| Data migration risk | Data-quality exceptions exceed threshold |
| Resource risk | Critical role vacancy remains open |
| Release risk | Critical defects remain open near deployment |

Early warning indicators help move risk management from reactive to proactive.

---

# Risk Response Strategies

Possible responses include:

```text id="risk-response"
Avoid
Mitigate
Transfer / Share
Accept
Escalate
```

The appropriate response depends on the organisation and the nature of the risk.

For each High or Critical risk, require:

```text id="risk-high-action"
Preventive action
Contingency action
Owner
Due date
Escalation trigger
```

---

# Mitigation vs Contingency

Keep these separate.

## Mitigation

Action taken **before** the risk materialises to reduce likelihood or impact.

Example:

> Complete an API compatibility proof of concept four weeks before SIT.

## Contingency

Action taken **if the risk occurs**.

Example:

> Use the approved temporary mock service to protect the SIT schedule.

---

# Risk Owner vs Action Owner

Do not automatically treat these as the same role.

**Risk Owner**

Accountable for monitoring and managing the overall risk.

**Action Owner**

Responsible for completing a specific mitigation action.

Example:

```text id="risk-owner-example"
Risk:
Security approval may delay production release.

Risk Owner:
Project Manager

Action:
Submit security evidence by 15 August.

Action Owner:
Security Lead
```

---

# Example Input

```text id="risk-example-input"
Project:
Customer Portal Implementation

Current Phase:
Integration Testing

Delivery Approach:
Hybrid Agile

Target Go-Live:
30 September 2027

Team:
Internal product team
External development vendor
External identity provider

Known Dependencies:
Identity API certification
CRM integration
Security approval
Business UAT

Known Issues:
Identity certification is 10 working days behind plan.
Two critical integration defects remain open.
Business tester availability for UAT is not yet confirmed.

Known Constraints:
Fixed September launch target.
Security review requires four weeks.
```

---

# Example Risk Register

| ID | Category | Risk | L | I | Score | Rating | Owner |
|---|---|---|---:|---:|---:|---|---|
| R-01 | Vendor | Identity-provider certification may miss the SIT dependency date | 4 | 4 | 16 | High | Integration Lead |
| R-02 | Quality | Critical integration defects may remain unresolved before UAT | 3 | 5 | 15 | High | QA Lead |
| R-03 | Resources | Insufficient business testers may delay UAT completion | 3 | 4 | 12 | High | Business Owner |
| R-04 | Security | Security evidence may not be ready for the four-week review window | 3 | 5 | 15 | High | Security Lead |

---

# Prompt 2 — Risk Prioritisation Review

After creating the register, run a management review.

```text id="risk-priority"
ROLE

You are a senior IT Project Manager reviewing the current project
risk exposure.

TASK

Review the risk register below and identify the five risks requiring
the highest level of management attention.

[PASTE RISK REGISTER]

Do not rank risks solely by numerical score.

Also consider:

- proximity,
- dependency impact,
- business impact,
- security / compliance impact,
- ability to recover,
- cross-project impact,
- vendor dependency,
- decision urgency.

OUTPUT FORMAT

Risk
Why Management Attention Is Required
Current Exposure
Immediate Action
Decision Required
Decision Owner
Decision Deadline
Escalation Trigger
```

---

# Risk Proximity

Consider when the risk could realistically affect the project.

Suggested classification:

```text id="risk-proximity"
Immediate
< 2 weeks

Near-term
2–6 weeks

Medium-term
6–12 weeks

Long-term
> 12 weeks
```

A Medium-rated risk that may materialise tomorrow can require more attention than a High-rated risk several months away.

---

# Risk Interdependency Review

For complex projects, assess whether risks are connected.

Example:

```text id="risk-chain"
Vendor API delay
↓
Integration testing delay
↓
UAT delay
↓
Business readiness compressed
↓
Go-live risk
```

Ask the AI to identify:

- risk chains,
- common root causes,
- correlated risks,
- risks that could trigger several other risks.

This is particularly useful in enterprise projects.

---

# Agile / Scrum Considerations

Risk identification may consider:

- backlog uncertainty,
- Sprint / iteration dependencies,
- technical debt,
- Product Owner availability,
- release readiness,
- team capacity,
- Definition of Done,
- cross-team integration.

Do not rely only on a static risk register.

Risks should also be surfaced through normal delivery feedback loops.

---

# Kanban Considerations

Where Kanban is used, relevant risk signals may include:

- increasing WIP,
- ageing work,
- blocked items,
- cycle-time deterioration,
- throughput decline,
- repeated Service Level Expectation breaches,
- bottlenecks.

These metrics may act as early warning indicators for delivery risk.

---

# Predictive Considerations

Risk review may be closely linked to:

- schedule milestones,
- critical path,
- budget,
- procurement,
- resource plans,
- formal change control.

---

# Hybrid Considerations

Combine formal risk governance with delivery-level indicators.

Example:

```text id="risk-hybrid"
Delivery signal
↓
Risk assessment
↓
Risk owner
↓
Mitigation
↓
Governance escalation if threshold exceeded
```

---

# Risk Escalation Criteria

Define explicit escalation triggers where practical.

Examples:

```text id="risk-escalation"
Risk rating becomes Critical.

Risk threatens a committed milestone.

Expected financial impact exceeds project tolerance.

Security or compliance exposure exceeds accepted tolerance.

Mitigation requires sponsor-level authority.

Risk affects more than one workstream.

Risk cannot be managed within the Project Manager's authority.
```

---

# Risk Review Questions

During each formal review ask:

```text id="risk-review-questions"
Has likelihood changed?

Has impact changed?

Has proximity changed?

Is the mitigation working?

Has the early warning indicator been triggered?

Has the risk become an issue?

Has a new dependency appeared?

Does the owner still have authority to manage the risk?

Does the risk require escalation?

Can the risk now be closed?
```

---

# Risk vs Issue

Keep risks and issues separate.

## Risk

An uncertain future event.

> There is a risk that the vendor may miss the API delivery date.

## Issue

Something that has already occurred.

> The vendor has missed the API delivery date by ten working days.

When a risk materialises, move it into the issue-management process rather than leaving it as an active future risk.

---

# Quality Checklist

Before accepting the risk register, confirm:

- [ ] Risks describe uncertain events
- [ ] Causes and impacts are explicit
- [ ] Likelihood is assessed
- [ ] Impact is assessed
- [ ] Significant risks have owners
- [ ] High/Critical risks have actions
- [ ] Early warning indicators exist
- [ ] Mitigation and contingency are separated
- [ ] Review dates are defined
- [ ] Risk proximity is considered
- [ ] Dependencies are considered
- [ ] Material risks have escalation criteria
- [ ] Existing issues are not incorrectly recorded as risks

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- uncertainty,
- risk identification,
- qualitative risk analysis,
- risk response,
- monitoring,
- stakeholder communication,
- governance,
- escalation.

## PMBOK Relevance

This prompt supports:

- risk,
- planning,
- governance,
- delivery,
- measurement,
- stakeholders.

## Delivery Framework

Framework-neutral.

Adaptable to:

- Predictive
- Agile
- Scrum
- Kanban
- Hybrid

---

# Human Review Required

Validate material risks with relevant stakeholders, including:

- Project Manager
- Risk Owner
- Business Owner
- Technical Lead
- Security
- QA
- Vendors
- Sponsor / Steering Committee where escalation is required

AI can assist with identifying patterns and structuring risk information.

It cannot determine the organisation's actual risk tolerance or accept project risk on behalf of accountable stakeholders.

---

# Confidentiality

Risk registers may contain highly sensitive information.

Do not enter into public AI tools:

- security vulnerabilities,
- confidential commercial exposure,
- vendor negotiation positions,
- personal performance information,
- sensitive customer information,
- protected financial exposure.

Anonymise information where required.

---

# Prompt Metadata

```text id="risk-metadata"
Prompt ID: RISK-001
Category: Risk & Issue Management
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Risk Owners / PMO / Sponsor
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: High
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT project risk-register framework |
