# Scope Definition and Gap Review

## Purpose

Use this framework to define project scope clearly and then audit it for ambiguity, missing requirements, ownership gaps, dependencies, and delivery risk.

The workflow has two steps:

1. **Draft the scope**
2. **Audit the scope**

The goal is to reduce:

- scope creep,
- conflicting stakeholder expectations,
- unclear responsibilities,
- missed dependencies,
- rework,
- and avoidable change requests.

---

## Best Used For

**Project phase:**  
Initiation / Early Planning

**Project type:**  
Software development / System implementation / Digital transformation / Data project / Integration project / Infrastructure initiative

**Primary user:**  
Project Manager / Project Coordinator / Business Analyst / Product Owner / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At project initiation and after major scope changes

---

# Prompt 1 — Draft the Scope

```text id="scope-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, requirements clarification, stakeholder alignment,
cross-functional coordination, and project governance.

TASK

Create a clear and structured scope definition for the project described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[BUSINESS OBJECTIVE]

Expected business value:
[VALUE / BENEFITS]

Current phase:
[INITIATION / PLANNING]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Primary users:
[USERS / BUSINESS UNITS]

Systems involved:
[LIST]

Known business processes:
[LIST]

Known requirements:
[LIST]

Known integrations:
[LIST]

Known dependencies:
[LIST]

Known constraints:
[LIST]

Known exclusions:
[LIST]

Known assumptions:
[LIST]

OUTPUT FORMAT

Create the following sections:

1. In Scope
2. Out of Scope
3. To Be Confirmed
4. Key Deliverables
5. System Interfaces
6. Business Responsibilities
7. Technical Responsibilities
8. Dependencies
9. Assumptions
10. Acceptance Criteria

Use precise, unambiguous language.

Each scope item should describe one clear responsibility,
deliverable, capability, boundary, or outcome.
```

---

# Prompt 2 — Scope Gap Audit

Run this prompt after Prompt 1.

```text id="scope-02"
ROLE

You are a senior IT Project Manager and Business Analyst reviewing
a project scope before detailed planning and delivery begin.

TASK

Audit the scope definition below.

Identify:

1. Ambiguous statements
2. Missing requirements
3. Missing deliverables
4. Unclear system interfaces
5. Unclear business responsibilities
6. Unclear technical responsibilities
7. Dependencies without owners
8. Scope items likely to generate future change requests
9. Requirements without measurable acceptance criteria
10. Items that should be explicitly out of scope
11. Assumptions that could materially affect delivery
12. Conflicts between business expectations and technical boundaries

SCOPE DEFINITION

[PASTE OUTPUT FROM PROMPT 1 HERE]

OUTPUT FORMAT

Provide a gap-analysis table:

Gap / Issue
Location in Scope
Why It Is a Risk
Potential Delivery Impact
Recommended Clarification
Owner
Priority
```

---

# Analysis Rules

When drafting or reviewing the scope:

1. Do not invent missing requirements.
2. Separate confirmed scope from assumptions.
3. Flag vague terms such as:
   - appropriate,
   - user-friendly,
   - seamless,
   - fast,
   - modern,
   - sufficient,
   - as required.
4. Identify responsibilities without an owner.
5. Identify integrations without clear ownership.
6. Flag requirements without measurable acceptance criteria.
7. Identify dependencies that could affect timeline or cost.
8. Highlight unclear boundaries between internal teams and vendors.
9. Distinguish deliverables from business outcomes.
10. Identify items that need sponsor or governance decisions.

---

# Delivery-Approach Considerations

Use these only where relevant.

## Agile / Scrum

Consider:

- product boundaries,
- backlog ownership,
- release scope,
- Minimum Viable Product,
- acceptance criteria,
- Definition of Done,
- evolving requirements.

## Kanban

Consider:

- service boundaries,
- classes of service,
- workflow ownership,
- operational demand,
- WIP policies,
- continuous intake of work,
- Service Level Expectations.

## Predictive

Consider:

- scope baseline,
- work packages,
- formal acceptance,
- milestone commitments,
- change-control implications.

## Hybrid

Consider how fixed commitments interact with iterative or flow-based delivery.

---

# Example Input

```text id="scope-example-input"
Project:
Customer Self-Service Portal

Business objective:
Reduce manual customer-service workload.

Expected value:
Lower service cost and faster response times.

Known requirements:
- Customers can log in.
- Customers can update contact details.
- Customers can download invoices.
- Customers can view payment status.
- Portal should be mobile friendly.

Systems involved:
CRM
Identity platform
Billing system

Known integrations:
CRM API
Billing API

Known constraints:
Go-live must happen before Q4 campaign.

Known exclusion:
Online contract cancellation is not included.

Open question:
It is not yet agreed whether customers can update bank details.
```

---

# Example Output Excerpt

## In Scope

1. Implement secure customer authentication using the existing identity platform.
2. Enable customers to view and update approved contact details.
3. Enable customers to download invoices from the billing system.
4. Display current payment status.
5. Provide responsive browser-based access for supported mobile and desktop devices.

## Out of Scope

1. Online contract cancellation.
2. Replacement of the existing CRM platform.
3. Replacement of the identity platform.

## To Be Confirmed

1. Whether customers may update bank details.
2. Whether payment history beyond current payment status is required.
3. Whether customer-service agents require an administration interface.

---

# Example Gap Analysis

| Gap / Issue | Why It Is a Risk | Recommended Clarification |
|---|---|---|
| “Mobile friendly” is not measurable | Different teams may interpret it differently | Define supported devices, browsers, and responsive acceptance criteria |
| Bank-detail updates unresolved | May materially affect security and scope | Sponsor and Security to confirm before design |
| CRM API ownership not stated | Integration delay may have no accountable owner | Assign API owner and delivery date |
| No performance requirement | Solution may work functionally but not at required scale | Define response-time and concurrent-user expectations |

---

# Scope Quality Checklist

Before approving the scope, confirm:

- [ ] In-scope items are explicit
- [ ] Out-of-scope items are explicit
- [ ] Unresolved items are visible
- [ ] Deliverables are defined
- [ ] Interfaces are identified
- [ ] Responsibilities have owners
- [ ] Dependencies are documented
- [ ] Acceptance criteria are measurable
- [ ] Vendor boundaries are clear
- [ ] Security responsibilities are clear
- [ ] Assumptions are visible
- [ ] No material ambiguity remains

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- scope definition,
- stakeholder alignment,
- requirements management,
- dependency management,
- change management,
- risk identification,
- governance.

## PMBOK Relevance

This prompt supports:

- scope,
- planning,
- stakeholders,
- governance,
- risk,
- value delivery.

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

The scope should be validated by relevant stakeholders, including:

- Project Sponsor
- Business Owner
- Product Owner where relevant
- Business Analyst
- Solution Architect
- Information Security
- QA / Test Lead
- External vendors where applicable

The scope is not considered approved until accountable stakeholders confirm the boundaries.

---

# Confidentiality

Do not include:

- customer personal data,
- employee personal data,
- credentials,
- passwords,
- API keys,
- confidential supplier pricing,
- confidential contract terms,
- proprietary architecture,
- security-sensitive technical details.

Use anonymised project information where required.

---

# Prompt Metadata

```text id="scope-metadata"
Prompt ID: INIT-003
Category: Project Initiation
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Business Owner / Business Analyst / Solution Architect
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
| 1.0 | YYYY-MM-DD | Initial IT scope definition and gap-review workflow |
