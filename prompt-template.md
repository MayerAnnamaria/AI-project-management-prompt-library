# Prompt Template

Use this template for every reusable prompt in the repository.

The objective is to make each prompt:

- clear,
- reusable,
- reviewable,
- professionally governed,
- and suitable for different project environments.

---

## 1. Prompt Name

**Example:** Risk Register Review

---

## 2. Business Purpose

Describe the project-management problem this prompt is designed to solve.

**Example:**

> Support the Project Manager in reviewing a project risk register, identifying weak or incomplete entries, and prioritising risks that require management attention.

---

## 3. Best Used For

**Project phase:**  
Initiation / Planning / Delivery / Testing / Deployment / Close-out

**Project type:**  
Small IT project / Enterprise IT project / Software implementation / Digital transformation / Data project

**Primary user:**  
Project Manager / Project Coordinator / PMO / Delivery Manager / Business Analyst

**Recommended frequency:**  
Ad hoc / Weekly / Monthly / Before steering committee / Before go-live

---

## 4. Professional Role

Define the perspective the AI should use.

### Template

```text id="zllrlq"
You are a senior IT Project Manager with experience delivering
complex software and digital transformation projects.

You have expertise in project planning, risk management,
stakeholder coordination, software delivery, quality assurance,
and project governance.
```

Adapt the role only when the task requires specialist expertise.

Examples:

- Senior Risk Manager
- Delivery Manager
- PMO Lead
- Business Analyst
- QA Manager
- Product Owner
- Vendor Manager

---

## 5. Task

Define **one primary task**.

### Template

```text id="m7iy3c"
TASK:

Review the project information below and identify the project risks
that require immediate management attention.
```

Avoid combining unrelated tasks into one prompt.

A good task should be:

- specific,
- measurable where possible,
- directly linked to a project decision,
- and clear about what the AI should analyse.

---

## 6. Project Context

Provide enough information for meaningful analysis.

### Template

```text id="pybdr5"
PROJECT CONTEXT:

Project:
[Project description]

Objective:
[Business objective]

Current phase:
[Initiation / Planning / Development / Testing / Deployment]

Delivery methodology:
[Agile / Scrum / Waterfall / Hybrid]

Timeline:
[Key dates and milestones]

Team:
[Team size and roles]

Stakeholders:
[Key stakeholders]

Current status:
[Green / Amber / Red]

Known risks or issues:
[List]

Dependencies:
[List]

Constraints:
[List]
```

Only include information relevant to the task.

Do not include confidential or sensitive project information in public AI tools.

---

## 7. Analysis Requirements

Specify how the AI should think about the problem.

### Example

```text id="vm988r"
For each risk:

1. Identify the underlying cause.
2. Describe the potential project impact.
3. Estimate probability.
4. Estimate severity.
5. Identify early warning indicators.
6. Recommend a mitigation action.
7. Assign an appropriate owner role.
8. Define when escalation is required.
```

This section converts a generic request into structured decision support.

---

## 8. Output Format

Always define the required output.

### Example

```text id="meao37"
OUTPUT FORMAT:

Provide a table with the following columns:

Risk ID
Risk Description
Root Cause
Probability
Impact
Risk Rating
Early Warning Indicator
Mitigation
Owner
Escalation Trigger
```

If an executive summary is required:

```text id="icqggb"
After the table provide:

1. Overall project risk assessment
2. Top three management priorities
3. Decisions required
```

---

## 9. Assumptions

Require assumptions to be explicit.

### Template

```text id="x7y4nh"
Do not invent missing project information.

Where information is unavailable:

- identify the gap,
- state the assumption separately,
- explain how the assumption affects the analysis.
```

This is especially important for professional project-management use.

---

## 10. Quality Review

Before accepting the AI output, verify:

- Are facts separated from assumptions?
- Are recommendations specific?
- Are owners defined?
- Are actions realistic?
- Are deadlines or escalation triggers included?
- Are risks linked to actual project context?
- Is the language suitable for the intended audience?
- Is anything presented as fact without supporting information?

---

## 11. Human Review Required

The Project Manager must review the result before use.

Human validation is mandatory when the output affects:

- project budget,
- contractual commitments,
- scope decisions,
- risk acceptance,
- staffing,
- client communication,
- executive reporting,
- security,
- production deployment,
- or go-live approval.

---

## 12. Confidentiality Check

Before submitting project information to an AI tool, remove or anonymise:

- customer names,
- employee personal data,
- passwords,
- credentials,
- API keys,
- confidential financial information,
- commercially sensitive pricing,
- confidential contractual information,
- proprietary technical architecture,
- security-sensitive information.

---

## 13. Example Input

Provide a short fictional example.

```text id="w0t8xp"
Project:
Customer self-service portal implementation

Phase:
System integration testing

Team:
1 Project Manager
1 Product Owner
5 Developers
2 QA Engineers

Current status:
Amber

Known issue:
Payment API integration is two weeks behind schedule.

Dependency:
External payment provider must complete certification before UAT.
```

---

## 14. Example Output

Include a short example showing what good output looks like.

| Risk | Impact | Recommended Action | Owner |
|---|---|---|---|
| Payment API certification delay | UAT start may slip | Escalate certification timeline with supplier and create fallback test plan | Integration Lead |

Examples should remain fictional and concise.

---

## 15. Prompt Metadata

Every reusable prompt should include:

```text id="83f2fe"
Prompt ID:
Category:
Version:
Status:
Owner:
Reviewer:
Created:
Last Reviewed:
Project Type:
Risk Level:
AI Model Tested:
```

### Status values

```text id="w2v462"
Draft
Tested
Reviewed
Approved
Retired
```

---

## 16. Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial version |
| 1.1 | YYYY-MM-DD | Improved output structure |
| 1.2 | YYYY-MM-DD | Added governance and review criteria |

---

## Standard Prompt Structure

Every prompt in this repository should follow this sequence:

```text id="d81wv4"
ROLE
↓
TASK
↓
CONTEXT
↓
ANALYSIS REQUIREMENTS
↓
OUTPUT FORMAT
↓
ASSUMPTIONS
↓
QUALITY CHECK
↓
HUMAN REVIEW
```

The purpose of the structure is consistency.

A reusable professional prompt should not only generate an answer.

It should help the Project Manager produce a **structured, reviewable and actionable decision-support output**.
