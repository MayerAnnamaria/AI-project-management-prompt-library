# SMART Project Objectives

## Purpose

Use this prompt to convert high-level project goals into clear, measurable, and accountable SMART objectives.

SMART objectives help connect:

- business value,
- project scope,
- success criteria,
- delivery priorities,
- KPIs,
- ownership,
- and governance.

The objective is not only to define what the project will deliver, but also how success will be measured.

---

## Best Used For

**Project phase:**  
Initiation / Planning

**Project type:**  
Software development / System implementation / Digital transformation / Data project / Process improvement / Product initiative

**Primary user:**  
Project Manager / Project Coordinator / Delivery Manager / PMO / Business Analyst / Product Owner

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At initiation and after major strategic or scope changes

---

# Prompt

```text
ROLE

You are a senior IT Project Manager experienced in international
software delivery, digital transformation, stakeholder management,
business analysis, and project governance.

TASK

Create SMART project objectives for the project described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business problem:
[BUSINESS PROBLEM]

Strategic purpose:
[WHY THE PROJECT EXISTS]

Expected business value:
[EXPECTED BENEFITS]

Target completion:
[DATE]

Budget:
[BUDGET OR RANGE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Key stakeholders:
[LIST]

Expected business outcomes:
[LIST]

Known constraints:
[LIST]

Known dependencies:
[LIST]

Known success criteria:
[LIST]

OUTPUT FORMAT

Create 5 SMART project objectives.

For each objective provide:

1. Objective statement
2. Specific outcome
3. Measurement method
4. Target value
5. Target date
6. Accountable owner
7. Related business benefit
8. Primary dependency
9. Key risk to achievement
```

---

# SMART Quality Criteria

Each objective should be:

## Specific

The objective should clearly describe what must be achieved.

## Measurable

The result should be objectively measurable.

## Achievable

The target should be realistic given the available time, budget, resources, and constraints.

## Relevant

The objective should directly support the project's business purpose.

## Time-Bound

The objective should have a defined target date or review period.

---

# Analysis Rules

When creating the objectives:

1. Do not invent unsupported targets.
2. Flag missing baselines.
3. Identify objectives that depend on unresolved scope.
4. Identify objectives that rely heavily on vendors or external teams.
5. Separate project outputs from business outcomes.
6. Avoid vague language such as:
   - improve significantly,
   - enhance user experience,
   - optimise processes,
   - increase efficiency,
   - deliver high quality.
7. Convert vague goals into measurable outcomes where the available information allows.
8. If a measurable target is missing, state:
   **Target to be confirmed.**
9. Identify dependencies that may prevent achievement.
10. Highlight objectives that conflict with project constraints.

---

# Delivery-Approach Considerations

Use only where relevant.

## Agile / Scrum

Consider:

- product goals,
- incremental value delivery,
- release objectives,
- user outcomes,
- Product Owner accountability,
- measurable acceptance criteria.

## Kanban

Consider:

- service-level objectives,
- flow improvement,
- lead time,
- cycle time,
- throughput,
- service quality,
- operational outcomes.

## Predictive

Consider:

- milestone achievement,
- planned benefits,
- schedule commitments,
- budget commitments,
- formal acceptance criteria.

## Hybrid

Consider both fixed business commitments and iterative or flow-based delivery outcomes.

---

# Example Input

```text
Project:
Customer Self-Service Portal

Business Problem:
Customer Service receives a high volume of manual account-management requests.

Strategic Purpose:
Reduce operational workload and improve customer access to routine services.

Expected Business Value:
Lower service cost
Faster customer response times
Higher digital adoption

Target Completion:
30 September 2027

Budget:
€750,000

Delivery Approach:
Hybrid Agile

Known Constraints:
External development vendor
Legacy CRM API
Fixed September launch target

Expected Outcomes:
More customer requests handled digitally
Lower email volume
Improved service response
```

---

# Example Output

| Objective | Measurement | Target | Date | Owner |
|---|---|---|---|---|
| Launch the customer portal | Production deployment completed and approved | Successful go-live | 30 Sep 2027 | Project Manager |
| Increase digital handling of eligible requests | Share of eligible requests completed online | Target to be confirmed | 6 months after go-live | Customer Operations |
| Reduce manual service workload | Volume of eligible email requests | Target to be confirmed | 6 months after go-live | Customer Service Manager |
| Achieve production quality readiness | Open Severity 1 defects | 0 at go-live | Before release | QA Lead |
| Achieve operational readiness | Training, support model, and procedures approved | 100% complete | Before go-live | Operations Lead |

---

# Objective Quality Review

After creating the objectives, review each one.

Provide:

| Objective | SMART Rating | Weakness | Recommended Improvement |
|---|---|---|---|

Use:

```text
Strong
Acceptable
Needs Clarification
Not SMART
```

---

# Output vs Outcome Check

Classify each objective as:

```text
Project Output
Business Outcome
Operational Outcome
Quality Outcome
Flow / Delivery Outcome
```

Example:

| Objective | Type |
|---|---|
| Deploy CRM to production | Project Output |
| Reduce customer response time | Business Outcome |
| Train support team | Operational Outcome |
| Achieve zero Severity 1 defects | Quality Outcome |
| Reduce average cycle time | Flow / Delivery Outcome |

A strong project should normally include more than delivery-only objectives.

---

# Dependency Review

For each objective, identify:

```text
Objective
Primary Dependency
Dependency Owner
Risk if Dependency Fails
```

This prevents objectives from being treated as isolated targets.

---

# Quality Checklist

Before approving the objectives, confirm:

- [ ] Every objective supports the business case
- [ ] Every objective is measurable
- [ ] Every objective has an accountable owner
- [ ] Every objective has a target date
- [ ] Targets are evidence-based
- [ ] Outputs and outcomes are both represented
- [ ] Dependencies are visible
- [ ] Key risks are visible
- [ ] Vague wording has been removed
- [ ] Unsupported figures have not been invented

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- business value,
- benefits realization,
- stakeholder alignment,
- planning,
- measurement,
- accountability,
- delivery objectives.

## PMBOK Relevance

This prompt supports:

- value delivery,
- planning,
- measurement,
- stakeholders,
- governance,
- accountability.

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

Validate project objectives with:

- Project Sponsor
- Business Owner
- Product Owner where relevant
- Finance where financial benefits are involved
- IT leadership where technical commitments are involved
- Operations where post-launch benefits are expected

The sponsor and business owner should confirm that the objectives represent the agreed definition of project success.

---

# Confidentiality

Do not include:

- confidential financial targets,
- sensitive customer information,
- personal data,
- proprietary commercial targets,
- protected contract information,
- security-sensitive information.

Use anonymised values where required.

---

# Prompt Metadata

```text
Prompt ID: INIT-005
Category: Project Initiation
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Sponsor / Business Owner
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
| 1.0 | YYYY-MM-DD | Initial SMART objectives framework |
