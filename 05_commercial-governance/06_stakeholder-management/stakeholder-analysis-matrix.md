# Stakeholder Analysis Matrix

## Purpose

Use this prompt to identify, assess, and prioritise stakeholders for an IT, software, digital transformation, data, infrastructure, or technology-enabled project.

The analysis should help the Project Manager understand:

- who can influence the project,
- who is affected by it,
- what each stakeholder cares about,
- how much power and interest they have,
- whether their attitude is supportive or resistant,
- and how engagement should be adapted.

The objective is not simply to create a stakeholder list.

The objective is to understand **where stakeholder attention and management effort should be focused**.

---

## Best Used For

**Project phase:**  
Initiation / Planning / Delivery / Major Change

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / PMO / Business Analyst / Change Lead

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At initiation and reviewed throughout the project

---

# Prompt

```text id="stakeholder-analysis-01"
ROLE

You are a senior IT Project Manager experienced in stakeholder
management, international software delivery, organisational change,
project governance, and cross-functional communication.

TASK

Create a complete stakeholder analysis matrix for the project
described below.

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

Project organisation:
[DETAILS]

Key stakeholders:
[LIST]

External vendors:
[LIST]

Affected business areas:
[LIST]

Countries / languages:
[LIST]

Known stakeholder concerns:
[LIST]

OUTPUT FORMAT

For each stakeholder provide:

1. Stakeholder Name / Group
2. Role / Relationship to Project
3. Primary Interest
4. Power Level: High / Medium / Low
5. Interest Level: High / Medium / Low
6. Current Attitude: Supportive / Neutral / Resistant / Unknown
7. Key Concerns
8. Engagement Strategy
9. Communication Method
10. Communication Frequency
11. Responsible Project Role

Format as a table.

After the table:

- identify the top 3 stakeholders requiring the most active management,
- explain why,
- highlight any stakeholder whose attitude may materially affect project success.
```

---

# Stakeholder Analysis Dimensions

For each stakeholder assess:

```text id="stakeholder-dimensions"
Power
Interest
Attitude
Influence
Impact
Decision Authority
Information Need
Change Impact
```

Do not assume that seniority alone determines stakeholder importance.

---

# 1. Primary Interest

Ask:

> What does this stakeholder most care about?

Possible interests include:

```text id="stakeholder-interests"
Business outcome

Budget

Schedule

Customer experience

Operational stability

Security

Compliance

Technical architecture

Team workload

Product value

Vendor performance

Data quality

User adoption
```

---

# Example

```text id="stakeholder-interest-example"
Stakeholder:
Head of Customer Service

Primary Interest:
The new CRM must improve agent efficiency without disrupting
customer-service operations during rollout.
```

---

# 2. Power Level

Use:

```text id="stakeholder-power"
High
Can approve, stop, materially change, fund, or escalate the project.

Medium
Can influence important delivery decisions or stakeholder behaviour.

Low
Limited formal authority over project direction.
```

Power may come from:

- decision authority,
- funding,
- specialist expertise,
- regulatory authority,
- operational control,
- organisational influence.

---

# 3. Interest Level

Use:

```text id="stakeholder-interest-level"
High
Project outcome directly affects the stakeholder.

Medium
Stakeholder is affected but not continuously engaged.

Low
Limited direct involvement or impact.
```

Power and interest should be assessed separately.

---

# Power / Interest Matrix

Use the classic four-quadrant view:

| Power | Interest | Suggested Approach |
|---|---|---|
| High | High | Manage Closely |
| High | Low | Keep Satisfied |
| Low | High | Keep Informed |
| Low | Low | Monitor |

This is a starting point, not a complete engagement strategy.

---

# 4. Current Attitude

Use:

```text id="stakeholder-attitude"
Supportive

Neutral

Resistant

Unknown
```

Do not infer attitude without evidence.

If uncertain:

> Unknown — validate through stakeholder engagement.

---

# Attitude Evidence

Possible evidence includes:

```text id="stakeholder-attitude-evidence"
Meeting behaviour

Decision history

Response times

Feedback

Escalations

Participation

Resource commitment

Survey feedback

Direct stakeholder conversation
```

Avoid labelling a stakeholder “resistant” because they challenge the project.

Challenge may reflect legitimate project risk.

---

# 5. Key Concerns

Identify what may influence stakeholder behaviour.

Examples:

```text id="stakeholder-concerns"
Budget impact

Loss of control

Operational disruption

Job-role change

Data privacy

Workload

Implementation risk

Technical complexity

Vendor dependency

Customer impact
```

Understanding concerns improves engagement quality.

---

# 6. Engagement Strategy

For each stakeholder, define a practical strategy.

### Weak

```text id="stakeholder-strategy-weak"
Communicate regularly.
```

### Better

```text id="stakeholder-strategy-good"
Engage the Customer Service Director in monthly readiness reviews
and provide early visibility of training, cutover, and operational
risks.

Escalate decisions affecting frontline operations before they enter
final release planning.
```

---

# Engagement Strategy Should Answer

```text id="stakeholder-strategy-questions"
What do they need?

When do they need it?

What concerns should we address?

What decisions do they control?

How should we involve them?
```

---

# 7. Communication Method

Possible channels include:

```text id="stakeholder-methods"
Steering Committee

1:1 meeting

Project status report

Workshop

Email

Teams / Slack

Dashboard

Demo

Sprint Review

Risk review

Vendor review

Training session
```

The communication method should match stakeholder needs.

---

# 8. Communication Frequency

Possible frequencies:

```text id="stakeholder-frequency"
Daily

Weekly

Biweekly

Monthly

Milestone-based

Event-driven

As required
```

Do not over-communicate stakeholders who need only periodic governance information.

---

# Example Stakeholder Matrix

| Stakeholder | Interest | Power | Interest Level | Attitude | Engagement |
|---|---|---|---|---|---|
| Executive Sponsor | Business value / budget | High | High | Supportive | Manage closely |
| Product Owner | Scope / priorities | High | High | Supportive | Continuous engagement |
| Security Lead | Security approval | High | Medium | Neutral | Early and milestone-based engagement |
| End Users | Usability / process change | Low | High | Unknown | Keep informed and involve in testing |
| Vendor | Delivery / commercial outcome | Medium | High | Supportive | Weekly delivery governance |

---

# Example Input

```text id="stakeholder-example-input"
Project:
CRM Replacement

Stakeholders:
Executive Sponsor
Customer Service Director
Product Owner
IT Architecture
Security
Data Team
CRM Implementation Vendor
Customer Service Agents
Operations
Finance

Known Context:
Sponsor strongly supports the programme.
Customer Service Director is concerned about operational disruption.
Security has not yet been fully engaged.
Vendor relationship is positive.
Customer Service agents have had limited communication about the change.
```

---

# Example Output Excerpt

| Stakeholder | Power | Interest | Attitude | Key Concern | Engagement Strategy |
|---|---|---|---|---|---|
| Executive Sponsor | High | High | Supportive | Business value / timeline | Monthly steering, decision escalation |
| Customer Service Director | High | High | Neutral | Operational disruption | Readiness reviews and early cutover planning |
| Security Lead | High | Medium | Unknown | Security compliance | Early design review and milestone approvals |
| Service Agents | Low | High | Unknown | Process / workload change | Demos, UAT involvement, training |

---

# Top 3 Stakeholder Review

After creating the matrix, identify the three stakeholders requiring the most active management.

Consider:

```text id="stakeholder-priority-factors"
High power

High interest

Decision authority

Resistance

Critical dependency ownership

Ability to delay project

Operational impact

Influence over others
```

Do not simply select the three most senior people.

---

# Stakeholder Priority Prompt

```text id="stakeholder-priority"
ROLE

You are a senior IT Project Manager reviewing stakeholder risk.

TASK

From the stakeholder matrix below, identify the three stakeholders
requiring the highest level of active management.

[PASTE MATRIX]

For each explain:

1. Why they are important
2. What could happen if engagement fails
3. What engagement action should happen next
4. Who should own the relationship
```

---

# Stakeholder Attitude Trend

Stakeholder positions can change.

Track:

| Stakeholder | Previous Attitude | Current Attitude | Trend | Reason |
|---|---|---|---|---|

Possible trends:

```text id="stakeholder-trend"
Improving

Stable

Deteriorating

Unknown
```

Example:

> Security moved from Neutral to Supportive after early technical workshops and agreement on the evidence required for production approval.

---

# Stakeholder Risk Signals

Possible warning indicators:

```text id="stakeholder-signals"
Repeated missed decisions

Reduced meeting participation

Delayed approvals

Repeated escalation

Resource commitments withdrawn

Negative feedback

Contradictory stakeholder instructions

New resistance to scope or timeline
```

These may indicate emerging stakeholder risk.

---

# Stakeholder Dependency Review

Some stakeholders own critical project dependencies.

Provide:

| Stakeholder | Dependency | Required By | Impact if Late |
|---|---|---|---|

Examples:

```text id="stakeholder-dependencies"
Business Owner
→ UAT resources

Security
→ Production approval

Architecture
→ Technical decision

Finance
→ Budget approval

Vendor
→ API delivery
```

---

# Stakeholder Influence Map

Where useful, assess informal influence.

Ask:

```text id="stakeholder-influence"
Who influences the Sponsor?

Who influences end-user opinion?

Who controls access to decision-makers?

Who can accelerate or block approvals?

Who has informal authority?
```

Do not assume the organisation chart tells the full story.

---

# Agile / Scrum Considerations

Relevant stakeholders may include:

- Product Owner,
- users,
- business sponsors,
- technical stakeholders,
- external teams.

Sprint Reviews and product demonstrations can support stakeholder engagement.

Do not treat Scrum events as the complete stakeholder-management strategy.

---

# Kanban Considerations

Stakeholder engagement may focus on:

- service expectations,
- priority policies,
- blocked dependencies,
- delivery predictability,
- SLE performance.

Stakeholders who frequently change priorities may materially affect flow.

---

# Predictive Considerations

Stakeholder management may align strongly with:

- milestone approvals,
- formal governance,
- scope decisions,
- change control,
- acceptance.

---

# Hybrid Considerations

Combine continuous product engagement with formal governance.

Example:

```text id="stakeholder-hybrid"
Delivery-level engagement
+
Executive governance
```

---

# International / Multicultural Considerations

Where relevant assess:

```text id="stakeholder-international"
Language

Time zone

Decision-making culture

Communication style

Local organisational norms

Availability
```

Avoid stereotyping based on nationality or culture.

Use observed stakeholder behaviour and confirmed communication needs.

---

# Stakeholder Review Cadence

Review the matrix:

```text id="stakeholder-review-cadence"
At project initiation

Before major milestones

After organisational change

After major escalation

When stakeholder attitude changes

During regular governance reviews
```

Stakeholder analysis should be dynamic.

---

# Prompt 2 — Stakeholder Gap Review

```text id="stakeholder-gap-review"
ROLE

You are a PMO Lead reviewing a stakeholder analysis.

TASK

Review the stakeholder matrix below.

[PASTE MATRIX]

Check for:

- missing decision-makers,
- missing end users,
- missing operational owners,
- missing technical stakeholders,
- missing security / compliance stakeholders,
- unvalidated attitudes,
- stakeholders with unclear engagement owners,
- high-power stakeholders with insufficient engagement.

OUTPUT FORMAT

Gap
Why It Matters
Potential Impact
Recommended Action
Priority
```

---

# Quality Checklist

Before approving the matrix, confirm:

- [ ] Key stakeholders are identified
- [ ] Business stakeholders are included
- [ ] Technical stakeholders are included
- [ ] Operations are included where relevant
- [ ] Vendors are included
- [ ] End users are considered
- [ ] Power is assessed
- [ ] Interest is assessed
- [ ] Attitude is assessed or marked unknown
- [ ] Key concerns are understood
- [ ] Engagement strategy is specific
- [ ] Communication method is defined
- [ ] Frequency is defined
- [ ] Top-priority stakeholders are identified
- [ ] Stakeholder attitudes will be reviewed over time

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- stakeholder identification,
- stakeholder analysis,
- engagement,
- communication,
- governance,
- leadership,
- change management.

## PMBOK Relevance

This prompt supports:

- stakeholders,
- team,
- governance,
- communication,
- delivery.

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

Stakeholder assessments should be reviewed by the Project Manager and relevant project leaders.

AI can:

- structure stakeholder information,
- identify potential gaps,
- suggest engagement approaches.

AI should not:

- infer stakeholder attitudes without evidence,
- make sensitive personal judgments,
- replace direct stakeholder engagement.

---

# Confidentiality

Stakeholder analysis may contain sensitive information.

Protect:

- stakeholder attitudes,
- internal influence,
- organisational conflicts,
- personal concerns,
- escalation history,
- political or commercial sensitivities.

Do not distribute the stakeholder matrix more widely than necessary.

---

# Prompt Metadata

```text id="stakeholder-analysis-metadata"
Prompt ID: STAKE-001
Category: Stakeholder Management
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: PMO / Sponsor
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Medium
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT stakeholder-analysis framework |
