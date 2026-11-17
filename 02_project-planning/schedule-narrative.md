# Schedule Narrative

## Purpose

Use this prompt to convert project milestones, delivery dates, dependencies, and planning data into a concise professional schedule narrative.

The narrative should explain:

- overall delivery timing,
- major phases or workstreams,
- key milestones,
- critical dependencies,
- sequencing logic,
- schedule risks,
- and recovery considerations.

The objective is not to repeat a Gantt chart in prose.

The objective is to explain the **logic behind the schedule**.

---

## Best Used For

**Project phase:**  
Planning / Delivery

**Project type:**  
Software implementation / Digital transformation / Data project / Infrastructure / ERP / System migration / Hybrid programme

**Primary user:**  
Project Manager / Project Coordinator / Delivery Manager / PMO

**Delivery approach:**  
Predictive / Hybrid / Agile where milestone-based reporting is required

**Recommended frequency:**  
At baseline planning, major re-planning events, and governance reporting

---

# Prompt

```text id="schedule-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, project planning, dependency management,
delivery governance, and executive reporting.

TASK

Write a professional schedule narrative from the project planning
information below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[BUSINESS OBJECTIVE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Planned start:
[DATE]

Target completion:
[DATE]

Major phases / workstreams:
[LIST]

Key milestones:
[LIST WITH DATES]

Critical dependencies:
[LIST]

External dependencies:
[LIST]

Known schedule risks:
[LIST]

Known constraints:
[LIST]

Current schedule status:
[ON TRACK / AT RISK / DELAYED]

Known variance:
[DETAILS]

Recovery actions:
[IF AVAILABLE]

OUTPUT FORMAT

Write a professional schedule narrative covering:

1. Overall timeline
2. Major phases or workstreams
3. Key milestones
4. Sequencing logic
5. Critical dependencies
6. Areas of overlap or parallel delivery
7. Current schedule risk
8. Recovery or mitigation approach
9. Key decisions required

Use concise professional language suitable for:

- project governance,
- steering committee reporting,
- PMO review,
- sponsor communication.
```

---

# Schedule Narrative Principles

A good schedule narrative should explain **why the dates matter**.

Avoid simply writing:

```text id="schedule-weak"
Requirements finish in March.
Development finishes in June.
Testing finishes in August.
Go-live is in September.
```

Prefer:

```text id="schedule-strong"
Requirements and solution design are planned to complete by the end
of March, enabling the core development phase to begin in April.

Integration work will overlap with configuration from May onward,
with system integration testing dependent on completion of the
CRM and identity-management interfaces.

UAT is planned for August and remains dependent on successful SIT
completion and business-user availability.

The September go-live therefore remains primarily exposed to
integration readiness and UAT completion.
```

---

# Critical Path / Critical Dependency Logic

Where applicable, identify the chain of activities that directly affects the target completion date.

For IT projects, this may include:

```text id="schedule-critical"
Requirements approval
↓
Solution design
↓
Build / configuration
↓
Integration
↓
System testing
↓
UAT
↓
Production readiness
↓
Go-live
```

However, do not automatically assume that every project follows this sequence.

Use the actual delivery context.

---

# Delivery-Approach Considerations

## Predictive

The narrative may focus on:

- baseline dates,
- critical path,
- milestone variance,
- schedule float,
- sequencing,
- recovery planning.

## Agile / Scrum

Focus on:

- release roadmap,
- Sprint or iteration cadence,
- major release goals,
- cross-team dependencies,
- backlog readiness,
- integration milestones.

Avoid treating Sprint plans as fixed long-term commitments.

## Kanban

Do not force flow-based delivery into a traditional milestone narrative.

Where relevant, focus on:

- service delivery expectations,
- major external commitments,
- flow constraints,
- blocked work,
- lead-time trends,
- delivery forecasts.

## Hybrid

Explain the relationship between:

- governance milestones,
- iterative delivery,
- release cadence,
- vendor commitments,
- regulatory or business deadlines.

---

# Dependency Analysis

For major dependencies, provide:

| Dependency | Required By | Owner | Current Status | Schedule Impact if Late |
|---|---|---|---|---|

Possible dependency types:

- Business
- Technical
- Vendor
- Security
- Data
- Infrastructure
- Regulatory
- Environment
- Resource

---

# Schedule Risk Review

After writing the narrative, identify the main threats to schedule performance.

Use:

| Schedule Risk | Cause | Potential Impact | Early Warning Indicator | Mitigation | Owner |
|---|---|---|---|---|---|

Focus on risks that can affect major milestones or delivery commitments.

---

# Example Input

```text id="schedule-example-input"
Project:
CRM Replacement

Delivery Approach:
Hybrid

Planned Start:
1 February 2027

Target Go-Live:
1 October 2027

Milestones:
Requirements approval — 31 March
Solution design approval — 30 April
Configuration complete — 30 June
System Integration Testing complete — 31 July
UAT complete — 31 August
Production readiness approval — 20 September
Go-live — 1 October

Dependencies:
CRM vendor configuration
Customer data migration
Telephony integration
Security approval
Business-user availability for UAT

Known Risk:
Data cleansing is two weeks behind plan.

Constraint:
Security review requires four weeks.
```

---

# Example Output

## Schedule Narrative

The CRM replacement programme is planned to run from February to October 2027, with production deployment targeted for 1 October.

Requirements approval is planned for the end of March, followed by solution-design approval at the end of April. Configuration and integration activities will proceed through June, with System Integration Testing scheduled for July.

UAT is planned for August and is dependent on successful completion of integration testing, sufficiently migrated test data, and business-user availability. Production readiness activities will then run through September, including final security approval and operational preparation.

The main schedule risk is currently associated with data cleansing, which is approximately two weeks behind plan. If this delay affects migration readiness for SIT or UAT, the October go-live could be placed at risk. The recovery plan should therefore prioritise data-quality remediation and confirm whether migration preparation can proceed in parallel with remaining cleansing activities.

---

# Schedule Health Classification

After the narrative, classify schedule health:

```text id="schedule-health"
GREEN
Major milestones achievable with current plan.

AMBER
Milestones remain achievable but require active management,
recovery actions, or resolution of material dependencies.

RED
Current plan is no longer achievable without re-baselining,
scope change, additional capacity, or governance intervention.
```

Provide the status and one-sentence rationale.

---

# Recovery Analysis

If the project is delayed or at risk, assess possible recovery options.

Examples:

```text id="schedule-recovery"
Parallelise eligible activities
Re-sequence work
Reduce dependency waiting time
Add temporary capacity
Prioritise critical deliverables
Defer non-critical scope
Accelerate vendor decisions
Resolve approval bottlenecks
Change release sequencing
```

For each recovery option identify:

| Option | Potential Benefit | Risk / Trade-Off | Decision Owner |
|---|---|---|---|

Do not recommend acceleration without identifying the corresponding risk.

---

# Quality Review

Before finalising the schedule narrative, verify:

- [ ] Dates are internally consistent
- [ ] Major milestones are included
- [ ] Dependencies are explicit
- [ ] Schedule risks are visible
- [ ] Assumptions are not presented as facts
- [ ] Parallel work is explained
- [ ] Critical delivery logic is understandable
- [ ] Variances are clearly stated
- [ ] Recovery actions are realistic
- [ ] Decision requirements are visible

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- schedule management,
- planning,
- dependency management,
- forecasting,
- risk management,
- stakeholder communication,
- governance.

## PMBOK Relevance

This prompt supports:

- planning,
- schedule,
- delivery,
- measurement,
- risk,
- governance.

## Delivery Framework

Adaptable to:

- Predictive
- Agile
- Scrum
- Kanban
- Hybrid

The level of schedule detail should match the delivery method.

---

# Human Review Required

Validate the narrative with relevant stakeholders, including:

- Project Manager
- Delivery Lead
- Technical Lead
- Product Owner where relevant
- QA Lead
- Vendor leads
- PMO
- Business Owner where business milestones are affected

AI-generated schedule commentary should never replace the approved schedule or source planning data.

---

# Confidentiality

Do not include:

- confidential contract dates where restricted,
- commercially sensitive vendor commitments,
- protected financial information,
- security-sensitive deployment information,
- personal data.

Use anonymised dates or project names where required.

---

# Prompt Metadata

```text id="schedule-metadata"
Prompt ID: PLAN-002
Category: Project Planning
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Delivery Lead / PMO
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Low
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT schedule narrative framework |
