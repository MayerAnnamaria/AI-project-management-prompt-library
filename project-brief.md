# Project Brief

## Purpose

Use this prompt to convert rough stakeholder notes, meeting outputs, or early project information into a structured IT project brief.

The project brief should give stakeholders a concise view of:

- why the project exists,
- what it is expected to deliver,
- what is included and excluded,
- what constraints and dependencies exist,
- and what needs clarification before planning begins.

---

## Best Used For

**Project phase:**  
Initiation

**Project type:**  
Software development / System implementation / Digital transformation / Data project / Process automation

**Primary user:**  
Project Manager / Project Coordinator / Business Analyst / PMO

**Recommended frequency:**  
At project initiation or when a new initiative is being evaluated

---

# Prompt

```text
ROLE

You are a senior IT Project Manager experienced in software delivery,
digital transformation, stakeholder management, requirements clarification,
and project governance.

TASK

Convert the raw project information below into a professional project brief.

PROJECT CONTEXT — RAW NOTES

[PASTE RAW NOTES HERE]

The notes may include:

- business problem,
- objectives,
- stakeholder requests,
- technical requirements,
- timelines,
- dependencies,
- assumptions,
- risks,
- constraints,
- vendor information,
- budget information,
- unresolved questions.

Do not invent missing information.

Where information is unclear or incomplete, flag it explicitly.

OUTPUT FORMAT

Create the project brief with the following sections:

1. Project Overview

Provide a concise summary of:

- business problem,
- project purpose,
- expected business value.

2. Project Objectives

List the main objectives.

Where possible, convert vague objectives into measurable statements.

Flag objectives that are not yet measurable.

3. Scope

Separate into:

IN SCOPE

OUT OF SCOPE

TO BE CONFIRMED

4. Key Deliverables

Provide:

Deliverable | Description | Expected Outcome | Owner | Target Date

5. Key Requirements

Separate into:

- Business requirements
- Functional requirements
- Technical requirements
- Security requirements
- Operational requirements

If a category is not supported by the available information, mark it as:
"Not yet defined."

6. Key Constraints

Assess:

- Timeline
- Budget
- Resources
- Technology
- Security
- Regulatory / Compliance
- Vendor availability
- Business availability

7. Dependencies

Provide:

Dependency | Type | Impact | Owner | Required By

8. Key Stakeholders

Provide:

Stakeholder | Role | Interest | Decision Authority | Engagement Need

9. High-Level Risks

Provide:

Risk | Cause | Potential Impact | Initial Response | Owner

10. Assumptions

Provide:

Assumption | Impact if Incorrect | Validation Required | Owner

11. Open Questions

List all unresolved questions that should be answered before detailed planning begins.

12. Recommended Next Steps

Provide the five most important actions required to move the project forward.
```

---

# Analysis Rules

When creating the project brief:

1. Preserve confirmed project facts.
2. Do not invent missing project information.
3. Separate facts from assumptions.
4. Identify contradictory information.
5. Highlight unclear scope boundaries.
6. Identify dependencies that could affect delivery.
7. Flag requirements that are too vague for planning.
8. Identify decisions that require sponsor or business-owner input.

---

# Example Input

```text
Need customer portal this year.

Customers currently email support for address changes, invoice copies,
payment-status questions and account updates.

Customer service says volume is too high.

IT says we can probably reuse existing login.

CRM API is old and may need changes.

Security must approve authentication.

External vendor can start development in March.

Budget approximately €500k but Finance has not confirmed final amount.

Target launch September.

Marketing wants mobile-friendly design.

Operations wants reporting dashboard.

No agreement yet about whether customers can change bank details online.
```

---

# Example Output Excerpt

## Project Overview

The proposed Customer Self-Service Portal aims to reduce manual customer-service workload by enabling customers to complete selected account-management activities online.

The project is expected to improve customer response times and reduce operational dependency on email-based support processes.

---

## Scope

### In Scope

- Customer authentication
- Address updates
- Invoice retrieval
- Payment-status visibility
- Mobile-responsive customer portal

### Out of Scope

No confirmed out-of-scope items have yet been identified.

### To Be Confirmed

- Online bank-detail changes
- Reporting dashboard scope
- CRM API enhancement requirements

---

## Open Questions

1. Is the €500k budget formally approved?
2. Which customer transactions require additional security controls?
3. Can the existing authentication solution support the required user volume?
4. Is the September launch date fixed or target-based?
5. Who has final authority over scope approval?

---

# Quality Review

Before using the project brief, confirm:

- [ ] Business problem is clearly stated
- [ ] Objectives are measurable
- [ ] Scope boundaries are explicit
- [ ] Major dependencies are identified
- [ ] Key stakeholders are included
- [ ] Open questions are visible
- [ ] No unsupported assumptions are presented as facts
- [ ] Recommended next steps are actionable

---

# Human Review Required

The Project Manager should validate the brief with:

- Project Sponsor
- Business Owner
- IT / Architecture
- Information Security
- Finance
- Product Owner or Business Analyst
- Relevant vendors

The brief should not be treated as approved project scope until accountable stakeholders confirm it.

---

# Confidentiality

Do not include:

- customer personal data,
- employee personal data,
- passwords,
- API keys,
- confidential supplier pricing,
- confidential contracts,
- proprietary architecture,
- security-sensitive technical details.

Use anonymised project information where required.

---

# Prompt Metadata

```text
Prompt ID: INIT-002
Category: Project Initiation
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Sponsor / PMO / Business Owner
Project Type: IT / Digital Transformation
Risk Level: Low
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT project brief framework |
