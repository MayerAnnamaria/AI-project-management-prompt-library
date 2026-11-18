# RACE Prompt Framework for Project Management

**Prompt ID:** AIFRM-001 | **Category:** AI Prompt Frameworks | **Version:** 1.2 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Structure AI requests to produce evidence-based management analysis, actionable recommendations, and professional stakeholder communication.

**When to use:** Project prioritization, scope changes, delivery risks, stakeholder management, executive reporting, and management decision support.

### The RACE Framework

| Element | Purpose |
|---|---|
| **R — Role** | Define the relevant professional expertise |
| **A — Ask** | Specify the management problem and decision |
| **C — Context** | Provide verified facts, constraints, and business priorities |
| **E — Expected Output** | Define the analysis, recommendation, and communication requirements |

### Copy-and-Paste Prompt

```text
ROLE

Act as a Senior IT Project Manager experienced in
international software delivery, stakeholder management,
scope control, risk management, and project governance.

Apply commercially aware, solution-oriented,
and assertive management judgment.

ASK

[DEFINE THE PRIMARY MANAGEMENT PROBLEM]

Objective:
[DESIRED MANAGEMENT OUTCOME]

Decision required:
[DECISION / NOT APPLICABLE]

CONTEXT

Project: [ANONYMIZED PROJECT NAME]
Business objective: [OBJECTIVE]
Delivery approach: [AGILE / PREDICTIVE / HYBRID]
Project phase: [PHASE]
Current status: [VERIFIED STATUS]
Release / milestone: [DATE OR TIMEFRAME]
Resources / capacity: [RELEVANT INTERNAL DATA]
Existing commitments: [SCOPE / DELIVERABLES]
New request / issue: [DESCRIPTION]
Business justification: [STAKEHOLDER REQUIREMENT]
Risks / dependencies: [LIST]
Constraints: [TIME / BUDGET / QUALITY / SCOPE]
Decision authority: [ROLE / NOT CONFIRMED]

Stakeholder audience:
[CLIENT / BUSINESS OWNER / SPONSOR / INTERNAL TEAM]

EXPECTED OUTPUT

1. EXECUTIVE SUMMARY
   Explain the management problem and business impact.

2. IMPACT ASSESSMENT
   Assess schedule, capacity, scope, quality,
   dependencies, and business consequences.

3. MANAGEMENT OPTIONS
   Present realistic options and trade-offs.

4. RECOMMENDATION
   Recommend one preferred option.
   Explain why it best protects business value
   and existing delivery commitments.

5. STAKEHOLDER COMMUNICATION
   Draft a concise, professional message
   appropriate for the specified audience.

6. REQUIRED ACTIONS
   Action | Proposed Owner | Expected Outcome

7. DECISION REQUIRED
   Specify the decision, approval authority,
   and unresolved information gaps.

STAKEHOLDER COMMUNICATION STANDARD

Use a confident, diplomatic, commercially aware,
and assertive senior project-management tone.

Structure the message as follows:

1. ACKNOWLEDGE
   Recognize the stakeholder's business priority
   without excessive praise or apologetic language.

2. EXPLAIN THE IMPLICATION
   Clearly describe how the request affects
   agreed scope, delivery commitments,
   business outcomes, or timelines.

3. STATE THE RECOMMENDATION
   Recommend a specific course of action.
   Be decisive without making unauthorized commitments.

4. PRESENT THE ALTERNATIVE
   If the stakeholder's requirement is business-critical,
   explain how alternative delivery options
   and associated trade-offs can be assessed.

5. DEFINE THE NEXT STEP
   Explain the required alignment,
   assessment, or approval process.

COMMUNICATION RULES

- Focus on business outcomes, not internal team problems.
- Do not disclose Jira board details, internal capacity
  calculations, staffing constraints, or defect data
  unless authorized and relevant to the recipient.
- Do not blame developers, suppliers, or stakeholders.
- Avoid vague phrases such as "we will try",
  "hopefully", or "we will do our best".
- Avoid unnecessary apologies or defensive explanations.
- Do not promise unapproved scope, dates, or resources.
- Use clear recommendations, not passive suggestions.
- Explain consequences without creating conflict.
- Keep customer-facing communication to 100–150 words
  unless more detail is explicitly required.
- Use natural business language, not corporate jargon.

ANALYSIS AND GOVERNANCE RULES

- Separate facts, assumptions, and recommendations.
- Quantify impacts where reliable data is available.
- Do not invent project metrics or commitments.
- Consider business value alongside delivery constraints.
- Distinguish internal analysis from external communication.
- Preserve formal decision and approval authority.
- Flag missing evidence affecting the recommendation.
```

### How to Use

1. **Define the decision:** Identify the specific project-management challenge.
2. **Provide the context:** Include internal delivery facts, stakeholder requirements, and project constraints.
3. **Specify the audience:** Clearly distinguish customer-facing communication from internal management reporting.
4. **Generate the analysis:** Review the options, quantified impacts, and recommendation.
5. **Validate the message:** Confirm that the stakeholder communication is business-focused, assertive, appropriate for disclosure, and aligned with approved commitments.

**Key distinction:** Internal management analysis may contain detailed capacity, resource, risk, and delivery information. Stakeholder communication should present only the relevant business implications and proposed path forward.

---

## 2. Quality Check

Use this independent prompt to evaluate both the management recommendation and the stakeholder communication.

```text
ROLE

You are an independent Senior PMO Reviewer
and Executive Communication Specialist.

TASK

Evaluate the RACE output for management quality,
business judgment, stakeholder communication,
and decision governance.

INPUT

[PASTE GENERATED RACE OUTPUT]

CHECK

1. MANAGEMENT ANALYSIS
   Are the main risks, constraints, and business
   implications accurately assessed?

2. RECOMMENDATION
   Is one preferred option clearly recommended
   with a sound business rationale?

3. BUSINESS ORIENTATION
   Does the response prioritize business outcomes
   and protect agreed delivery commitments?

4. ASSERTIVENESS
   Is the recommendation confident and decisive
   without being aggressive or inflexible?

5. STAKEHOLDER COMMUNICATION
   Is the message diplomatic, concise,
   professional, and solution-oriented?

6. INFORMATION DISCLOSURE
   Are unnecessary internal delivery details
   excluded from customer-facing communication?

7. NEXT STEPS
   Does the message identify a practical
   path toward alignment or approval?

8. GOVERNANCE
   Are recommendations distinguished from
   formally authorized decisions?

OUTPUT

Quality Verdict: PASS / REVISE

Score each dimension from 1–10:
- Professionalism
- Business Orientation
- Assertiveness
- Clarity
- Decision Readiness

Identify the three most important improvements.

If required, provide a revised stakeholder message
that addresses the weaknesses.

Do not invent missing facts, approvals,
or stakeholder commitments.
```

### Final Quality Checklist

- [ ] Clear management recommendation
- [ ] Business implications explained
- [ ] Relevant delivery trade-offs identified
- [ ] Assertive but diplomatic communication
- [ ] No unnecessary internal information disclosed
- [ ] Constructive alternative presented
- [ ] Specific next step defined
- [ ] Approval authority respected

---

## 3. Practical IT Use Case

### Competing Priorities — Urgent Scope Change vs. Release Deadline

**Scenario:** An Enterprise CRM Implementation is approaching release in four weeks.

The Sales Director requests a new Sales Performance Dashboard for the upcoming reporting cycle. However, the development team has limited available capacity, two high-priority defects remain unresolved, and the external vendor has not completed API certification.

The Project Manager must recommend whether to accept, defer, or reprioritize the request without jeopardizing existing delivery commitments.

### Project Context

| Attribute | Current Position |
|---|---|
| Project | Enterprise CRM Implementation |
| Delivery approach | Hybrid |
| Planned release | In 4 weeks |
| Remaining capacity | 40 person-days |
| Existing commitments | 35 person-days |
| Available buffer | 5 person-days |
| New request | Sales Performance Dashboard |
| Estimated effort | 12 person-days |
| Open defects | 2 High-priority |
| External dependency | Vendor API certification outstanding |
| Sponsor priority | Protect the release date |

### Example RACE Prompt

```text
ROLE

You are a Senior IT Project Manager experienced in
Hybrid delivery, scope control, stakeholder negotiation,
capacity planning, and risk management.

Use professional, commercially aware,
and assertive management communication.

ASK

Evaluate an urgent dashboard request competing
with existing CRM release commitments.

Recommend whether to accept, defer, or reprioritize
the request while protecting the release date.

CONTEXT

Project: Enterprise CRM Implementation
Release deadline: 4 weeks

Remaining capacity: 40 person-days
Existing commitments: 35 person-days
Available buffer: 5 person-days

New request:
Sales Performance Dashboard

Estimated effort:
12 person-days

Business justification:
The Sales Director considers the dashboard important
for the upcoming reporting cycle.

Current risks:
- 2 unresolved High-priority defects
- Vendor API certification outstanding
- No additional capacity confirmed

Sponsor priority:
Protect the committed release date.

Stakeholder audience:
Sales Director / Business Customer

EXPECTED OUTPUT

1. Executive Summary
2. Capacity and Delivery Impact
3. Three Management Options
4. Preferred Recommendation with Rationale
5. Professional Stakeholder Communication
6. Required Actions and Decision Authority

STAKEHOLDER COMMUNICATION REQUIREMENTS

Write a confident, diplomatic, business-focused
message suitable for the Sales Director.

- Acknowledge the business importance.
- Explain implications for agreed commitments.
- Recommend a clear course of action.
- Offer an alternative for critical requirements.
- Specify the decision and approval process.
- Do not disclose internal Jira, staffing,
  capacity calculations, or defect details.
- Do not blame the team or make unapproved promises.
- Avoid apologetic, vague, or defensive language.
- Limit the message to approximately 100–150 words.
```

### Example AI Output

#### Executive Summary

The additional dashboard requires an estimated 12 person-days, while only 5 person-days of unallocated capacity remain.

Including the dashboard without adjusting existing commitments would create a minimum capacity shortfall of **7 person-days** and increase schedule and quality exposure.

**Recommendation:** Defer the dashboard to the next release, subject to confirming its business criticality. If it must be delivered at launch, assess and approve a corresponding scope trade-off.

#### Capacity Impact

| Measure | Person-Days |
|---|---:|
| Remaining capacity | 40 |
| Existing commitments | 35 |
| Available buffer | 5 |
| Dashboard estimate | 12 |
| Total demand | 47 |
| Capacity shortfall | **7** |

*The calculation assumes the estimates are comparable and excludes additional unplanned defect or integration effort.*

#### Management Options

| Option | Business Benefit | Delivery Impact | Main Risk |
|---|---|---|---|
| **A. Accept now** | Dashboard delivered at launch | Exceeds available capacity | Release and quality exposure |
| **B. Defer** | Dashboard delivered in a later release | Protects current delivery commitments | Delayed business benefit |
| **C. Reprioritize** | Dashboard potentially delivered at launch | Requires scope substitution | Loss of previously committed functionality |

#### Recommended Management Decision

**Option B — Defer to the next release, subject to business-impact validation.**

This recommendation protects the current delivery commitments and avoids introducing additional scope while existing quality and integration risks remain unresolved.

If the dashboard is essential for the reporting cycle, Option C should be evaluated through formal change control.

### Stakeholder Communication

<text color="secondary" size="xs">Business/customer-facing message — excludes internal delivery capacity and Jira details.</text>

Thank you for clarifying the business importance of the dashboard for the upcoming reporting cycle.

We have assessed the request against the agreed release scope and delivery commitments. Including the additional functionality at this stage would require reprioritization of existing deliverables or an adjustment to the release timeline.

**My recommendation is to schedule the dashboard for the next release**, preserving the current delivery commitments and minimizing disruption to the implementation.

If the dashboard is essential for the upcoming reporting cycle, I propose reviewing its business priority together and identifying the scope trade-offs required to accommodate it. We can then submit the preferred option for approval through the established change control process.

### Required Management Actions

| Action | Proposed Owner | Required Outcome |
|---|---|---|
| Confirm business criticality | Sales Director / Product Owner | Establish whether launch delivery is essential |
| Validate effort and dependencies | Development Lead | Confirm delivery implications |
| Assess scope alternatives | Project Manager / Product Owner | Identify realistic trade-offs |
| Evaluate schedule and quality impact | Project Manager / QA Lead | Support informed decision-making |
| Review change options | Sponsor / Change Authority | Approve or reject proposed baseline changes |

### Applied Quality Review

| Criterion | Assessment |
|---|---|
| Professionalism | 9.5/10 |
| Business Orientation | 9.5/10 |
| Assertiveness | 9.5/10 |
| Clarity | 9.5/10 |
| Decision Readiness | 9/10 |

**Quality verdict: PASS — subject to management validation.**

The communication is confident, diplomatic, and business-focused. It provides a clear recommendation, recognizes the stakeholder's priority, and establishes a constructive path forward without disclosing unnecessary internal delivery information.

**Remaining validation:** Confirm the dashboard's business criticality, capacity assumptions, scope substitution options, and approval authority before changing project commitments.

### Management Value

This example demonstrates the ability to:

- Evaluate competing priorities using delivery evidence.
- Recommend a clear course of action.
- Communicate constraints without exposing internal project details.
- Manage stakeholder expectations constructively.
- Preserve scope control and formal decision authority.

**Key principle:** Effective stakeholder communication combines **clear recommendations, business-oriented reasoning, constructive alternatives, and accountable decision-making**.


