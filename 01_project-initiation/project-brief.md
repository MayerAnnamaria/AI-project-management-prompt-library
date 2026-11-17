# Project Brief

## Purpose

Use this prompt to convert early stakeholder input, rough project notes, meeting outputs, or incomplete business information into a structured IT project brief.

The project brief should provide enough clarity to support:

- initial stakeholder alignment,
- project evaluation,
- early scope discussion,
- delivery planning,
- governance setup,
- and identification of information gaps.

The brief is not a substitute for approved scope or a full project charter.

---

## Best Used For

**Project phase:**  
Initiation / Discovery

**Project type:**  
Software development / System implementation / Digital transformation / Data project / Infrastructure project / Product initiative

**Primary user:**  
Project Manager / Project Coordinator / Delivery Manager / Business Analyst / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At the start of a new initiative or when an existing initiative requires clarification

---

# Prompt

```text
ROLE

You are a senior IT Project Manager experienced in international
software delivery, digital transformation, stakeholder management,
requirements clarification, and project governance.

TASK

Convert the project information below into a structured professional project brief.

PROJECT CONTEXT — RAW INPUT

[PASTE PROJECT NOTES, MEETING NOTES, EMAIL SUMMARY, OR EARLY PROJECT INFORMATION HERE]

The input may include:

- business problem,
- strategic objective,
- expected business value,
- users,
- stakeholders,
- scope ideas,
- requirements,
- technical systems,
- timelines,
- budget information,
- dependencies,
- vendors,
- constraints,
- assumptions,
- risks,
- unresolved questions.

Do not invent missing project information.

Where information is incomplete, unclear, contradictory, or unconfirmed,
flag it explicitly.

OUTPUT FORMAT

Create the project brief using the following sections:

1. Project Overview

Summarise:

- the business problem,
- the proposed initiative,
- the intended outcome,
- the expected business value.

2. Project Objectives

List the known project objectives.

For each objective identify:

- objective,
- expected outcome,
- measurement method if available,
- owner if known.

Flag objectives that are not measurable.

3. High-Level Scope

Separate into:

IN SCOPE

OUT OF SCOPE

TO BE CONFIRMED

Do not infer scope boundaries that have not been agreed.

4. Key Deliverables

Provide:

Deliverable | Description | Expected Outcome | Owner | Target Date

5. Key Requirements

Group known requirements into:

- Business
- Functional
- Technical
- Data
- Security
- Operational
- Compliance

Where a category is not supported by the available information,
state:

"Not yet defined."

6. Key Constraints

Assess known constraints across:

- Schedule
- Budget
- Resources
- Technology
- Security
- Compliance
- Vendor availability
- Business availability
- Operational environment

7. Key Dependencies

Provide:

Dependency
Type
Potential Impact
Owner
Required By
Status

8. Key Stakeholders

Provide:

Stakeholder
Role
Primary Interest
Decision Authority
Engagement Requirement

9. High-Level Risks

Provide:

Risk
Cause
Potential Impact
Initial Response
Owner

10. Assumptions

Provide:

Assumption
Reason
Impact if Incorrect
Validation Required
Owner

11. Delivery Approach Considerations

Based only on the available information, identify any considerations
relevant to the stated delivery approach.

Do not recommend changing methodology unless there is clear evidence.

12. Open Questions

List unresolved questions that should be answered before detailed
planning or delivery begins.

13. Recommended Next Steps

Identify the five most important actions required to move the initiative forward.
```

---

# Delivery-Approach Considerations

Use this section only where relevant.

## Agile / Scrum

Consider:

- product vision,
- Product Owner,
- backlog ownership,
- incremental delivery,
- release objectives,
- user feedback,
- Definition of Done.

## Kanban

Consider:

- service delivery objective,
- incoming demand,
- workflow,
- WIP policy,
- classes of service,
- Service Level Expectations,
- flow constraints.

## Predictive

Consider:

- scope baseline,
- schedule baseline,
- milestone commitments,
- critical dependencies,
- formal change control.

## Hybrid

Consider the interaction between fixed governance commitments and iterative or flow-based delivery.

---

# Analysis Rules

When creating the brief:

1. Preserve confirmed facts.
2. Do not invent missing information.
3. Separate facts from assumptions.
4. Flag contradictions.
5. Highlight unclear scope.
6. Identify unresolved ownership.
7. Identify dependencies that could affect delivery.
8. Flag requirements that are too vague for planning.
9. Distinguish business outcomes from project outputs.
10. Highlight missing governance decisions.

---

# Example Input

```text
Need customer portal this year.

Customers currently email support for address changes, invoice copies,
payment-status questions, and account updates.

Customer Service says volume is too high.

IT says existing login may be reusable.

CRM API is old and may need changes.

Security must approve authentication.

External development partner can start in March.

Budget approximately €500k but Finance has not confirmed final amount.

Target launch September.

Marketing wants mobile-friendly design.

Operations wants reporting dashboard.

No agreement yet about whether customers can change bank details online.
```

---

# Example Output Excerpt

## Project Overview

The proposed Customer Self-Service Portal is intended to reduce manual customer-service demand by enabling customers to complete selected routine account activities digitally.

The expected business value includes reduced service workload, faster response times, and improved digital access for customers.

---

## High-Level Scope

### In Scope

- Customer authentication
- Address updates
- Invoice retrieval
- Payment-status visibility
- Mobile-responsive customer portal

### Out of Scope

No confirmed out-of-scope items are available from the current information.

### To Be Confirmed

- Online bank-detail changes
- Reporting dashboard scope
- Required CRM API enhancements

---

## Open Questions

1. Is the €500k budget formally approved?
2. Is the September launch date fixed or target-based?
3. Can the existing authentication platform support the required user volume?
4. Who has final authority over scope approval?
5. Is the reporting dashboard part of the initial release or a later phase?

---

# Quality Review

Before using the brief, confirm:

- [ ] Business problem is clearly stated
- [ ] Expected value is visible
- [ ] Objectives are understandable
- [ ] Scope boundaries are visible
- [ ] Major dependencies are identified
- [ ] Key stakeholders are included
- [ ] Assumptions are separated from facts
- [ ] Open questions are explicit
- [ ] No unsupported details were invented
- [ ] Recommended actions are actionable

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- stakeholder identification,
- business value,
- project initiation,
- scope clarification,
- risk identification,
- governance,
- delivery planning.

## PMBOK Relevance

This prompt supports early project definition around:

- value,
- stakeholders,
- scope,
- planning,
- risk,
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

Validate the brief with relevant stakeholders, including:

- Project Sponsor
- Business Owner
- Product Owner where relevant
- Business Analyst
- IT / Architecture
- Information Security
- Finance
- Vendor representatives where applicable

The brief should not be treated as approved scope until accountable stakeholders confirm it.

---

# Confidentiality

Do not include:

- personal data,
- customer-identifying information,
- passwords,
- credentials,
- API keys,
- confidential supplier pricing,
- confidential contract terms,
- proprietary technical architecture,
- security-sensitive details.

Anonymise project information where required.

---

# Prompt Metadata

```text
Prompt ID: INIT-002
Category: Project Initiation
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Sponsor / Business Owner / PMO
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
| 1.0 | YYYY-MM-DD | Initial IT project brief framework |
