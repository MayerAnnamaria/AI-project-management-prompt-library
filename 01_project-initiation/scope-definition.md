# Scope Definition

## Purpose

Use this framework to define project scope clearly and then audit it for gaps, ambiguity, missing responsibilities, and delivery risk.

The workflow has two steps:

1. Draft the scope
2. Review the scope for gaps

This reduces the risk of scope creep, conflicting expectations, missed dependencies, and unclear ownership.

---

## Best Used For

**Project phase:**  
Initiation / Early Planning

**Project type:**  
Software development / System implementation / Digital transformation / Data project / Integration project

**Primary user:**  
Project Manager / Business Analyst / Product Owner / PMO

**Recommended frequency:**  
At project initiation and whenever major scope changes are proposed

---

# Prompt 1 — Draft the Scope

```text id="scope-01"
ROLE

You are a senior IT Project Manager experienced in software implementation,
requirements clarification, cross-functional delivery, stakeholder management,
and project governance.

TASK

Create a clear and structured scope definition for the project described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[BUSINESS OBJECTIVE]

Current phase:
[INITIATION / PLANNING]

Primary users:
[USERS / BUSINESS UNITS]

Systems involved:
[LIST]

Business processes affected:
[LIST]

Known requirements:
[LIST]

Known integrations:
[LIST]

Known constraints:
[LIST]

Known exclusions:
[LIST]

Known dependencies:
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
8. Assumptions
9. Dependencies
10. Acceptance Criteria

Use precise, unambiguous language.

Each scope item should describe one clear responsibility, deliverable, or boundary.
```

---

# Prompt 2 — Scope Gap Audit

Run this prompt after Prompt 1.

```text id="scope-02"
ROLE

You are a senior IT Project Manager and Business Analyst reviewing a project
scope before detailed planning and delivery begin.

TASK

Audit the scope definition below.

Identify:

1. Ambiguous statements
2. Missing requirements
3. Missing deliverables
4. Unclear system interfaces
5. Unclear business responsibilities
6. Unclear technical responsibilities
7. Dependencies that are not assigned
8. Scope items that could lead to change requests later
9. Requirements that lack measurable acceptance criteria
10. Items that should be explicitly listed as out of scope

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
3. Flag vague words such as:
   - appropriate,
   - sufficient,
   - user-friendly,
   - fast,
   - modern,
   - seamless,
   - as required.
4. Identify responsibilities that have no clear owner.
5. Identify integrations without defined ownership.
6. Flag requirements without acceptance criteria.
7. Highlight dependencies that could affect timeline or cost.
8. Identify boundaries between internal teams and external vendors.

---

# Example Input

```text id="scope-example-input"
Project:
Customer Self-Service Portal

Business objective:
Reduce manual customer-service workload.

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

# Example Scope Output

## In Scope

1. Implement secure customer authentication using the existing identity platform.
2. Enable customers to view and update approved contact details.
3. Enable customers to download invoices from the billing system.
4. Display current payment status.
5. Provide responsive browser-based access for mobile and desktop devices.

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
| "Mobile friendly" is not measurable | Different teams may interpret it differently | Define supported devices, browsers, and responsive acceptance criteria |
| Bank-detail updates unresolved | May materially affect security and scope | Sponsor and Security to confirm before design |
| CRM API ownership not stated | Integration delays may have no accountable owner | Assign API owner and delivery date |
| No performance requirement | Portal may technically work but fail under expected load | Define expected concurrent-user volume and response-time target |

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
- [ ] No material ambiguity remains

---

# Human Review Required

The scope should be validated by relevant stakeholders, including:

- Project Sponsor
- Business Owner
- Product Owner
- Business Analyst
- Solution Architect
- Information Security
- QA / Test Lead
- External vendors where applicable

The scope is not considered approved until accountable stakeholders confirm the boundaries.

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
Risk Level: Medium
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT scope definition and gap-audit workflow |
