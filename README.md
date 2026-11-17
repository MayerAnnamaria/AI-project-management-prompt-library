# AI Project Management Playbook

A practical library of AI-assisted frameworks, prompts, and decision-support templates for IT project managers.

The purpose of this repository is not to replace professional project management judgement. It demonstrates how AI can be used systematically to support planning, delivery, risk management, stakeholder communication, reporting, quality assurance, and project governance.

The playbook is designed for modern IT delivery environments and can be adapted to predictive, Agile, hybrid, Scrum, or Kanban-based ways of working where appropriate.

---

## Why This Repository Exists

Project managers work with large volumes of information:

- project plans,
- risks and issues,
- stakeholder expectations,
- meeting notes,
- change requests,
- testing results,
- status reports,
- delivery dependencies,
- and executive decisions.

AI can help structure and analyse this information, but only when the task, context, expected output, and review criteria are clearly defined.

This repository provides reusable frameworks that turn ad-hoc prompting into a structured project-management workflow.

---

## Core Principle

> AI supports project management decisions.  
> The Project Manager remains accountable for the decision.

Every framework in this repository follows three principles:

1. **Provide sufficient project context**
2. **Define the expected decision or output clearly**
3. **Review and validate AI-generated results before use**

---

## What the Playbook Covers

### 1. Project Initiation

Frameworks for defining the project before delivery begins.

Examples:

- Project charter
- Project brief
- Scope definition
- Assumptions and constraints
- SMART objectives

---

### 2. Project Planning

Frameworks for translating objectives into an executable delivery approach.

Examples:

- Work Breakdown Structure
- Milestone planning
- Dependency analysis
- RACI matrix
- Resource planning
- Communication planning
- Release or iteration planning where relevant

---

### 3. Risk & Issue Management

Structured approaches for identifying, assessing, monitoring, and mitigating uncertainty.

Examples:

- Risk identification
- Risk register
- Qualitative risk analysis
- Mitigation planning
- Issue analysis
- RAID review

---

### 4. Delivery Management

Frameworks for identifying blockers, delivery risks, and execution problems.

Examples:

- Sprint health check
- Flow health check
- Blocker analysis
- Dependency review
- Delivery delay analysis
- Change impact analysis
- Release readiness

---

### 5. Reporting & Communication

Reusable frameworks for transforming project information into clear management communication.

Examples:

- Weekly status report
- Monthly project report
- Executive summary
- Steering committee update
- Escalation communication
- Lessons learned

---

### 6. Stakeholder Management

Frameworks for understanding stakeholder influence, expectations, and engagement needs.

Examples:

- Stakeholder analysis
- Power-interest matrix
- Stakeholder engagement plan
- Difficult stakeholder analysis
- Conflict resolution

---

### 7. Commercial & Project Governance

Decision-support frameworks for managing scope, cost, suppliers, and project controls.

Examples:

- Change request analysis
- Budget variance analysis
- Vendor performance review
- Scope gap analysis
- Commercial impact assessment

---

### 8. Quality & Testing

Frameworks for software quality, testing coordination, and release decisions.

Examples:

- Test strategy review
- UAT readiness
- Defect triage
- Root cause analysis
- Go-live readiness

---

### 9. Advanced AI Workflows

Techniques for using AI beyond single prompts.

Examples:

- Document audit
- Multi-step analysis
- Critical review
- Prompt chaining

---

### 10. AI Governance

Controls for responsible AI use in professional project environments.

Examples:

- Confidentiality checklist
- Hallucination check
- Human review checklist
- Responsible AI principles

---

# Prompt Design Framework

Prompts in this repository follow a structured approach based on four elements:

## Role

Define the professional perspective required.

Example:

> You are a senior IT Project Manager responsible for an international software implementation.

---

## Ask

Define one clear task.

Example:

> Analyse the current project risks and identify the five risks requiring immediate management attention.

---

## Context

Provide relevant project information.

Typical context may include:

- project objective,
- current phase,
- project size,
- delivery methodology,
- timeline,
- budget,
- team structure,
- dependencies,
- known risks,
- stakeholder concerns.

---

## Expected Output

Define the structure of the result.

Example:

| Risk | Root Cause | Probability | Impact | Mitigation | Owner | Deadline |
|---|---|---|---|---|---|---|

Clear output instructions improve consistency and make AI-generated results easier to review.

---

# Small vs Enterprise Projects

The same project-management problem may require different levels of analysis depending on project complexity.

## Small IT Project

Typical characteristics:

- 4–10 team members
- one development team
- limited external dependencies
- short delivery cycle
- small stakeholder group

Recommended output:

- concise
- operational
- action-oriented

---

## International Enterprise Project

Typical characteristics:

- multiple teams or workstreams
- several countries or time zones
- external vendors
- complex dependencies
- executive governance
- commercial constraints
- security or regulatory requirements

Recommended output:

- structured analysis
- explicit assumptions
- dependency assessment
- risk ownership
- escalation criteria
- decision deadlines
- governance impact

---

# Standard Prompt Structure

Each reusable prompt should contain:

```text
Business Problem
↓
Professional Role
↓
Task
↓
Project Context
↓
Required Analysis
↓
Output Format
↓
Quality Review
↓
Governance Considerations
```

---

# Example

Instead of asking:

> What are the risks in my project?

A structured project-management prompt would ask:

> Review the project context below and identify the five risks requiring immediate management attention.
>
> For each risk, identify:
>
> - underlying cause,
> - probability,
> - project impact,
> - early warning indicator,
> - mitigation action,
> - owner,
> - decision deadline.
>
> Separate confirmed facts from assumptions.

The goal is not simply better AI output.

The goal is **better structured project thinking**.

---

# Standards and Delivery Framework Alignment

Individual prompts in this repository may reference established project-management and delivery practices where relevant.

These may include:

- PMI and PMP-relevant project-management concepts
- Agile delivery principles
- Scrum practices
- Kanban flow-management concepts
- hybrid delivery models
- software quality and testing practices
- governance and stakeholder-management standards

The repository itself remains framework-neutral so that each prompt can be adapted to the actual delivery environment.

---

# AI Governance

AI-generated project-management content must be reviewed before use.

Do not enter confidential information into public AI tools.

Examples include:

- passwords or credentials,
- personal information,
- confidential customer information,
- commercially sensitive project data,
- contractual information,
- proprietary financial data,
- security-sensitive architecture.

AI-generated recommendations should also be independently reviewed before they influence:

- budget decisions,
- contractual decisions,
- risk acceptance,
- staffing decisions,
- executive reporting,
- production release,
- go-live decisions.

---

# Repository Philosophy

This repository treats prompts as reusable project-management assets.

A mature prompt is not simply a question.

It should have:

- a defined business purpose,
- clear inputs,
- expected outputs,
- quality criteria,
- an owner,
- version control,
- and professional review.

This approach allows AI-assisted project management to evolve from individual experimentation into a repeatable and governable working method.

---

# Intended Audience

This playbook is designed for:

- IT Project Managers
- Project Coordinators
- Delivery Managers
- PMO professionals
- Business Analysts
- Product Owners
- Software delivery teams
- professionals exploring responsible AI use in project management

---

# Disclaimer

The frameworks in this repository are intended for professional learning and decision support.

AI-generated outputs should never be treated as automatically correct.

The Project Manager remains responsible for validating information, reviewing assumptions, and making the final professional judgement.
