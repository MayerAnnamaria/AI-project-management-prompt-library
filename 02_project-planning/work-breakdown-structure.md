# Work Breakdown Structure

## Purpose

Use this prompt to break a project into a structured hierarchy of manageable deliverables, work packages, and activities.

A well-designed Work Breakdown Structure helps support:

- scope clarity,
- scheduling,
- ownership,
- dependency analysis,
- estimating,
- resource planning,
- risk identification,
- and progress tracking.

The objective is to create a structure that is detailed enough for planning without turning the WBS into an unmanageable task list.

---

## Best Used For

**Project phase:**  
Planning

**Project type:**  
Software implementation / Digital transformation / Data project / Infrastructure project / ERP / System migration / Product initiative

**Primary user:**  
Project Manager / Project Coordinator / Delivery Manager / PMO

**Delivery approach:**  
Predictive / Hybrid / Agile where WBS-style planning is useful

**Recommended frequency:**  
During initial planning and after major scope changes

---

# Prompt

```text id="wbs-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, digital transformation, project planning,
dependency management, and project governance.

TASK

Create a structured 3-level Work Breakdown Structure for the project described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[BUSINESS OBJECTIVE]

Project type:
[SOFTWARE / DATA / INFRASTRUCTURE / ERP / DIGITAL TRANSFORMATION / OTHER]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Key deliverables:
[LIST]

Known workstreams:
[LIST]

Known systems:
[LIST]

Known integrations:
[LIST]

Known dependencies:
[LIST]

Known vendors:
[LIST]

Known milestones:
[LIST]

Known constraints:
[LIST]

OUTPUT FORMAT

Create a 3-level WBS hierarchy.

Level 1:
Major project phases or workstreams

Level 2:
Major deliverables or work packages

Level 3:
Key planning-level activities or sub-deliverables

Use WBS coding:

1.0
1.1
1.1.1

Use an indented list format.

For each Level 2 work package, include:

- primary owner,
- major dependency,
- main completion criterion.

Do not create an excessively detailed task list.
```

---

# WBS Design Principles

The WBS should primarily be **deliverable-oriented**.

Prefer:

```text id="wbs-good"
3.2 CRM Integration
    3.2.1 Interface specification
    3.2.2 API development
    3.2.3 Integration testing
    3.2.4 Production readiness
```

Avoid vague structures such as:

```text id="wbs-bad"
3.2 CRM Work
    3.2.1 Meetings
    3.2.2 Emails
    3.2.3 Discussions
```

The WBS should describe project work that contributes to an identifiable result.

---

# Example Level 1 Structure

For a typical IT implementation, Level 1 might include:

```text id="wbs-level1"
1.0 Project Management and Governance
2.0 Discovery and Requirements
3.0 Solution Design
4.0 Build and Configuration
5.0 Integration
6.0 Data Migration
7.0 Testing and Quality Assurance
8.0 Security and Compliance
9.0 Business Readiness
10.0 Deployment and Go-Live
11.0 Hypercare and Transition
12.0 Project Close-Out
```

This is an example only.

The structure should be adapted to the actual project.

---

# Delivery-Approach Considerations

## Predictive

A WBS may be directly linked to:

- schedule activities,
- cost estimates,
- work packages,
- resource assignments,
- milestones,
- baselines.

## Agile / Scrum

Use the WBS at a higher level where useful.

For example:

```text id="wbs-agile"
Level 1:
Product / Delivery Area

Level 2:
Epic / Major Capability

Level 3:
Feature / Release Component
```

Do not replace the product backlog with an unnecessarily detailed WBS.

Use backlog decomposition where that is the better planning mechanism.

## Kanban

Use the WBS only for higher-level project or initiative decomposition where useful.

Day-to-day delivery should normally remain flow-based rather than being forced into a detailed hierarchical plan.

## Hybrid

A common approach is:

```text id="wbs-hybrid"
WBS
↓
Major deliverables
↓
Release / workstream planning
↓
Backlog or flow-based execution
```

This allows governance-level planning and adaptive delivery to coexist.

---

# WBS Gap-Check Prompt

After generating the first WBS, run a second review.

```text id="wbs-gap"
ROLE

You are a senior IT Project Manager performing a planning quality review.

TASK

Review the Work Breakdown Structure below and identify work that may be missing.

WBS

[PASTE WBS HERE]

Check specifically for missing work related to:

- project governance,
- requirements,
- architecture,
- environments,
- integrations,
- data,
- security,
- testing,
- UAT,
- deployment,
- rollback,
- business readiness,
- training,
- documentation,
- operational support,
- vendor coordination,
- compliance,
- transition,
- project close-out.

OUTPUT FORMAT

Provide:

Missing Work Package
Why It May Be Required
Potential Impact if Omitted
Recommended WBS Location
Priority
```

---

# Analysis Rules

When creating or reviewing the WBS:

1. Do not invent project scope.
2. Use the confirmed project scope as the primary boundary.
3. Flag potential work packages separately if they are not confirmed.
4. Do not confuse deliverables with organisational departments.
5. Avoid duplicate work across branches.
6. Identify interfaces between workstreams.
7. Include project-management and governance work where relevant.
8. Include testing and operational transition.
9. Include external vendor work where relevant.
10. Ensure every major deliverable can be mapped back to the project scope.

---

# Example Input

```text id="wbs-example-input"
Project:
CRM Replacement

Business Objective:
Replace the legacy CRM and migrate customer-service operations
to a modern cloud-based platform.

Delivery Approach:
Hybrid

Key Deliverables:
Configured CRM
Customer data migration
Email integration
Telephony integration
User training
Production deployment

Known Workstreams:
Business Analysis
CRM Configuration
Integrations
Data Migration
Testing
Change Management

Known Vendors:
CRM implementation partner
Data migration vendor

Known Milestones:
Design approval
Configuration complete
SIT complete
UAT complete
Go-live
```

---

# Example Output Excerpt

```text id="wbs-example-output"
1.0 Project Management and Governance
    1.1 Project Governance
        1.1.1 Governance structure confirmed
        1.1.2 Steering committee cadence established
        1.1.3 Decision and escalation process established

2.0 Discovery and Requirements
    2.1 Business Requirements
        2.1.1 Customer-service processes documented
        2.1.2 Functional requirements agreed
        2.1.3 Non-functional requirements agreed

3.0 Solution Design
    3.1 CRM Solution Design
        3.1.1 Configuration design
        3.1.2 Security design
        3.1.3 Integration design

4.0 CRM Configuration
    4.1 Core Platform Configuration
        4.1.1 User roles configured
        4.1.2 Case-management workflow configured
        4.1.3 Reporting configuration completed
```

---

# WBS Quality Review

Check the generated WBS against the following:

- [ ] All major scope areas are represented
- [ ] Work is grouped logically
- [ ] Deliverables are visible
- [ ] No major duplicate branches exist
- [ ] Level 2 work packages have clear ownership
- [ ] Major dependencies are visible
- [ ] Testing is included
- [ ] Security is included where relevant
- [ ] Data migration is included where relevant
- [ ] Deployment is included
- [ ] Operational transition is included
- [ ] Close-out is included
- [ ] Unconfirmed work is clearly marked

---

# WBS to Schedule Review

After creating the WBS, identify which Level 2 and Level 3 elements should feed into detailed scheduling.

Provide:

| WBS ID | Work Package | Schedule Required? | Key Dependency | Milestone |
|---|---|---|---|---|

Do not automatically turn every WBS item into a schedule activity.

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- scope decomposition,
- planning,
- schedule development,
- cost estimation,
- resource planning,
- dependency management,
- governance.

## PMBOK Relevance

This prompt supports:

- scope,
- planning,
- delivery,
- measurement,
- governance.

## Delivery Framework

Primarily useful for:

- Predictive
- Hybrid

Can also support:

- Agile
- Scrum
- Kanban

at higher levels where hierarchical decomposition adds value.

---

# Human Review Required

Validate the WBS with relevant stakeholders, including:

- Project Manager
- Business Analyst
- Solution Architect
- Technical Lead
- QA Lead
- Product Owner where relevant
- Vendor leads
- PMO where applicable

The WBS should be treated as a planning artifact, not as automatically approved project scope.

---

# Confidentiality

Do not include:

- sensitive architecture details,
- credentials,
- API keys,
- confidential supplier pricing,
- protected contract information,
- security-sensitive implementation details,
- personal data.

---

# Prompt Metadata

```text id="wbs-metadata"
Prompt ID: PLAN-001
Category: Project Planning
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Technical Lead / Business Analyst / PMO
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
| 1.0 | YYYY-MM-DD | Initial IT Work Breakdown Structure framework |
