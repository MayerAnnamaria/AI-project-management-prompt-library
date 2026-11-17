# Risk Identification Workshop

## Purpose

Use this prompt to prepare and facilitate a structured risk-identification workshop for an IT or digital project.

The AI-generated output should be treated as a **discussion seed list**, not as the project's final risk register.

The objective is to:

- help participants think broadly,
- avoid starting from a blank page,
- surface cross-functional risks,
- expose assumptions and dependencies,
- and create a stronger input for the formal risk register.

---

## Best Used For

**Project phase:**  
Initiation / Planning / Major Replanning / Pre-Release

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Multi-vendor programme

**Primary user:**  
Project Manager / Delivery Manager / Risk Facilitator / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At initiation and before major delivery or governance milestones

---

# Prompt 1 — Generate the Workshop Seed List

```text
ROLE

You are a senior IT Project Manager and risk facilitator experienced
in international software delivery, digital transformation,
cross-functional risk management, and project governance.

TASK

Create a risk-identification seed list for the project described below.

The list will be used as a starting point for a facilitated project
risk workshop.

It must prompt discussion rather than imply that all project risks
have already been identified.

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

Project team:
[DETAILS]

Systems involved:
[LIST]

External vendors:
[LIST]

Known dependencies:
[LIST]

Known assumptions:
[LIST]

Known constraints:
[LIST]

Known issues:
[LIST]

Risk domains to consider:
[LIST OR USE RELEVANT IT DOMAINS BELOW]

OUTPUT FORMAT

Organise the seed list by risk domain.

For each domain:

- provide 4–6 potential risks,
- use open-ended cause-event-impact wording,
- avoid assigning probability or impact scores,
- avoid presenting the list as complete,
- include 2–3 workshop questions that should provoke discussion.
```

---

# Suggested IT Risk Domains

Use only those relevant to the project.

```text
Business / Product
Scope / Requirements
Architecture
Technology
Integration
Data
Security
Privacy / Compliance
Infrastructure / Cloud
Testing / Quality
Release / Deployment
Operations / Support
Resources / Skills
Vendors / Procurement
Schedule
Budget
Stakeholders
Change Management
Governance
External Dependencies
```

For a smaller project, combine domains where appropriate.

For a large international programme, separate them further by workstream, platform, region, or supplier.

---

# Risk Phrasing

Use open-ended risk statements that encourage discussion.

### Weak

```text
API risk.
```

### Better

```text
Risk that the external API specification changes after integration
development has begun, creating rework and affecting the planned
integration-testing window.
```

### Better Workshop Style

```text
Could changes to the external API specification occur after
development begins, and if so, what would be the impact on
integration, testing, and release timing?
```

Workshop language should encourage participants to challenge assumptions.

---

# Example Risk Domains

## Architecture

Possible discussion starters:

```text
Risk that the target architecture contains unresolved design
decisions that delay development.

Risk that the proposed solution cannot meet expected transaction
volumes without redesign.

Risk that architecture dependencies between teams are not
identified early enough.
```

Workshop questions:

```text
Which architecture decisions remain unresolved?

Which technical assumptions have not yet been validated?

What architectural dependency could become a late-stage blocker?
```

---

## Integration

Possible discussion starters:

```text
Risk that external API delivery is later than required by the
integration schedule.

Risk that interface responsibilities between internal and vendor
teams are unclear.

Risk that test environments do not accurately represent production
integration behaviour.
```

Workshop questions:

```text
Which integration dependency has the least schedule flexibility?

Who owns each interface end-to-end?

Which external dependency do we currently have the least control over?
```

---

## Data

Possible discussion starters:

```text
Risk that source-data quality is lower than assumed, increasing
migration effort.

Risk that required data mappings are not approved before migration
development begins.

Risk that reconciliation criteria are not agreed before test migration.
```

Workshop questions:

```text
Which data-quality assumptions remain untested?

Who owns migration acceptance?

What would prevent us from proving that migrated data is correct?
```

---

## Security

Possible discussion starters:

```text
Risk that security requirements are identified too late to be
incorporated without significant rework.

Risk that penetration testing identifies release-blocking findings
close to deployment.

Risk that a third-party supplier does not meet required security
controls.
```

Workshop questions:

```text
Which security approvals could affect the critical delivery path?

When will security evidence be available?

Which security dependency sits outside the project team's control?
```

---

## Testing and Quality

Possible discussion starters:

```text
Risk that insufficient test-environment stability reduces effective
testing time.

Risk that critical defects remain unresolved when UAT begins.

Risk that acceptance criteria are too ambiguous for consistent testing.
```

Workshop questions:

```text
What could prevent us from completing meaningful testing?

Which quality assumptions are currently unsupported by evidence?

Where could defects escape into later stages?
```

---

## Vendors

Possible discussion starters:

```text
Risk that a strategic vendor cannot provide the planned delivery
capacity.

Risk that supplier responsibilities are interpreted differently by
internal and external teams.

Risk that commercial change-control delays technical decisions.
```

Workshop questions:

```text
Which deliverables depend on a single supplier?

What happens if the vendor misses its next major commitment?

Where are contract boundaries creating delivery ambiguity?
```

---

# Prompt 2 — Workshop Agenda

```text
ROLE

You are a senior IT Project Manager facilitating a cross-functional
risk workshop.

TASK

Create a 90-minute risk-identification workshop agenda using the
project context and seed list below.

PROJECT CONTEXT

[PASTE CONTEXT]

RISK SEED LIST

[PASTE SEED LIST]

OUTPUT FORMAT

Provide:

Time
Activity
Purpose
Facilitator Action
Participant Output
```

---

# Example Workshop Agenda

| Time | Activity | Purpose |
|---|---|---|
| 0–10 min | Context and objectives | Align participants |
| 10–20 min | Existing risks and assumptions | Establish baseline |
| 20–55 min | Domain-based risk identification | Generate risks |
| 55–70 min | Cross-team dependencies | Identify systemic risks |
| 70–80 min | Consolidation | Remove duplication |
| 80–90 min | Owners and next steps | Prepare for assessment |

Do not spend the workshop scoring every risk before adequate identification has occurred.

---

# Prompt 3 — Workshop Questions

Use prompts that challenge the project from different perspectives.

```text
What assumptions are we relying on that have not been validated?

What dependency could fail without us seeing it early?

Where do two teams believe the other team owns the same responsibility?

What important project outcome depends on a single person or supplier?

What could prevent testing from starting on time?

What could make the current release plan unrealistic?

What security or compliance requirement may still be unknown?

What could materially increase project cost?

Which stakeholder decision could arrive too late?

What would cause us to regret the current delivery approach?
```

---

# Pre-Workshop Preparation

Send participants the project context and seed list in advance.

Ask each domain or workstream lead to add risks specific to their area before the workshop.

Recommended inputs:

```text
Current scope
Project plan / roadmap
Architecture overview
Known dependencies
Assumptions register
Existing RAID register
Vendor commitments
Testing strategy
Release plan
Relevant metrics
```

The seed list should make preparation easier, not constrain participant thinking.

---

# Workshop Facilitation Rules

During the session:

1. Capture risks before debating solutions.
2. Avoid dismissing low-probability risks too quickly.
3. Distinguish risks from current issues.
4. Ask for causes and impacts.
5. Identify cross-team dependencies.
6. Record assumptions exposed during discussion.
7. Avoid assigning ownership before the risk is understood.
8. Combine duplicates only after discussion.
9. Do not let the AI-generated seed list define the boundaries of the workshop.
10. Encourage participants to add risks that were not anticipated.

---

# Risk vs Issue Check

Use:

```text
Has the event already happened?

YES → Issue
NO → Risk
```

Example:

```text
Risk:
The vendor may miss the API delivery date.

Issue:
The vendor has already missed the API delivery date.
```

---

# Prompt 4 — Consolidate Workshop Output

After the workshop:

```text
ROLE

You are a senior project risk manager consolidating the output
from a cross-functional IT risk workshop.

TASK

Clean and structure the workshop notes below.

WORKSHOP NOTES

[PASTE NOTES]

Do not remove unique risks simply because they appear similar.

Combine risks only where they clearly represent the same
cause-event-impact relationship.

OUTPUT FORMAT

Risk ID
Risk Category
Risk Statement
Cause
Potential Impact
Source / Workstream
Suggested Risk Owner
Information Required Before Scoring
```

---

# Cross-Functional Risk Review

After consolidation, specifically look for risks that cross multiple areas.

Example:

```text
Vendor delay
↓
Integration delay
↓
Testing compression
↓
Defect risk
↓
Release readiness risk
```

These are often more significant than isolated departmental risks.

Provide:

| Cross-Functional Risk | Affected Areas | Common Root Cause | Management Concern |
|---|---|---|---|

---

# Agile / Scrum Considerations

Where relevant, workshop discussion may include:

- backlog uncertainty,
- Product Owner availability,
- technical debt,
- release dependencies,
- cross-team dependencies,
- Definition of Done,
- integration frequency,
- team capacity.

Risk workshops should complement normal Agile feedback loops rather than replace them.

---

# Kanban Considerations

Use flow data as evidence during risk identification.

Possible signals include:

```text
Increasing WIP
Ageing work
Blocked items
Cycle-time deterioration
Throughput decline
Repeated SLE breaches
Persistent bottlenecks
```

Ask:

> What future delivery risk might this flow signal be warning us about?

Do not treat every metric change as a risk without understanding the underlying cause.

---

# Predictive Considerations

Use planning information such as:

- critical path,
- milestone dependencies,
- procurement lead times,
- resource plan,
- cost baseline,
- scope baseline.

---

# Hybrid Considerations

Review both:

```text
Formal project commitments
+
Adaptive delivery signals
```

A hybrid project may have delivery flexibility while still carrying fixed external dates, budgets, or governance obligations.

---

# Workshop Output

The final workshop should produce:

```text
Candidate risks
↓
Consolidated risks
↓
Validated risk statements
↓
Risk scoring
↓
Risk responses
↓
Risk owners
↓
Risk register
```

The workshop is an input into risk management, not the final step.

---

# Quality Checklist

Before closing the workshop, confirm:

- [ ] Multiple disciplines or perspectives participated
- [ ] AI seed list was treated only as a starting point
- [ ] New participant-generated risks were captured
- [ ] Risks are distinct from issues
- [ ] Causes and impacts are understandable
- [ ] Cross-team dependencies were considered
- [ ] Assumptions were challenged
- [ ] Vendor risks were considered
- [ ] Security and operational risks were considered where relevant
- [ ] Duplicate risks were reviewed carefully
- [ ] Follow-up actions are assigned
- [ ] Risks requiring further evidence are identified

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- risk identification,
- facilitation,
- stakeholder engagement,
- team collaboration,
- uncertainty management,
- dependency management,
- governance.

## PMBOK Relevance

This prompt supports:

- risk,
- stakeholders,
- planning,
- governance,
- delivery,
- team collaboration.

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

The workshop must remain a human collaborative process.

AI can:

- generate starting questions,
- structure risk statements,
- detect patterns,
- consolidate notes.

AI should not:

- decide which risks participants are allowed to discuss,
- independently approve risk ratings,
- assign final risk ownership,
- determine organisational risk tolerance.

---

# Confidentiality

Risk workshops can surface sensitive project information.

Protect:

- security vulnerabilities,
- commercially sensitive vendor concerns,
- personal performance information,
- confidential financial exposure,
- customer information,
- regulatory concerns.

Anonymise information before using public AI tools where required.

---

# Prompt Metadata

```text
Prompt ID: RISK-002
Category: Risk & Issue Management
Version: 1.0
Status: Draft
Owner: Project Manager / Risk Facilitator
Reviewer: Risk Owners / PMO
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
| 1.0 | YYYY-MM-DD | Initial IT risk-identification workshop framework |
