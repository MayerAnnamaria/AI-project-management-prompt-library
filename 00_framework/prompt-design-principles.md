# Prompt Design Principles

This repository follows a consistent set of prompt-design principles to ensure that AI-supported project-management work is structured, reusable, reviewable, and appropriate for professional delivery environments.

The objective is not to make prompts unnecessarily complex.

The objective is to make them useful for real project decisions.

---

# 1. Start With the Business Problem

A prompt should exist because there is a project-management problem to solve.

Avoid starting with:

> What can AI generate?

Start with:

> What decision, risk, issue, or management need must be addressed?

### Example

Weak framing:

```text
Create a risk table.
```

Better framing:

```text
The Project Manager needs to determine which current risks
require immediate escalation and whether existing mitigation
actions are sufficient.
```

This keeps the prompt focused on project value.

---

# 2. Define a Relevant Professional Role

Avoid generic roles.

### Weak

```text
You are a project manager.
```

### Better

```text
You are a senior IT Project Manager experienced in international
software delivery, stakeholder management, risk management,
quality assurance, and project governance.
```

For specialist tasks, use a specialist role.

Examples:

- Delivery Manager
- PMO Lead
- Business Analyst
- Risk Manager
- Product Owner
- Scrum Master
- Kanban Delivery Lead
- QA Manager
- Vendor Manager
- Solution Architect

### Principle

Use the most relevant professional perspective.

Do not automatically choose the most senior title.

---

# 3. One Primary Task per Prompt

Avoid combining unrelated tasks.

### Weak

```text
Review the risks, create a status report, write an escalation email,
and create a stakeholder matrix.
```

### Better

Use separate prompts for:

1. Risk analysis
2. Status reporting
3. Escalation communication
4. Stakeholder analysis

This improves:

- output quality,
- reusability,
- reviewability,
- testing,
- and version control.

---

# 4. Make the Ask Specific

Avoid vague instructions.

### Weak

```text
Analyse this project.
```

### Better

```text
Identify the five delivery risks most likely to affect the planned
production release within the next eight weeks.
```

A strong task should clarify:

- what should be analysed,
- what time horizon matters,
- what decision it supports,
- and what result is required.

---

# 5. Provide Relevant Context

AI output becomes more useful when the delivery environment is clear.

Relevant context may include:

- project objective,
- project phase,
- delivery approach,
- timeline,
- budget,
- team structure,
- stakeholders,
- vendors,
- dependencies,
- current status,
- known risks,
- known issues,
- relevant metrics,
- technical constraints,
- regulatory constraints.

Do not add information simply to make the prompt look detailed.

Only include information that can materially influence the analysis.

---

# 6. Adapt Context to the Delivery Framework

The core prompt structure can remain the same while the context changes.

## Agile / Scrum

Relevant context may include:

- Sprint Goal
- backlog status
- velocity
- blocked items
- acceptance criteria
- Definition of Done
- release target

## Kanban

Relevant context may include:

- WIP
- WIP limits
- cycle time
- lead time
- throughput
- work item age
- blocked work
- Service Level Expectation

## Predictive

Relevant context may include:

- baseline schedule
- critical path
- milestone variance
- cost variance
- change requests

## Hybrid

Relevant context may combine:

- fixed governance milestones
- iterative delivery
- release cadence
- external commitments
- cross-team dependencies

### Principle

Adapt the prompt to the actual project environment.

Do not force the project into a framework that does not fit.

---

# 7. Define the Output Format

Do not leave the structure entirely to the AI.

### Example

```text
OUTPUT FORMAT

Provide a table with:

Risk
Root Cause
Probability
Impact
Mitigation
Owner
Due Date
Escalation Trigger
```

Possible outputs include:

- tables,
- action lists,
- executive summaries,
- decision logs,
- stakeholder maps,
- structured reports,
- escalation messages,
- risk registers.

The format should match the intended audience.

---

# 8. Separate Facts From Assumptions

AI should not silently fill gaps.

Use instructions such as:

```text
Do not invent missing project information.

Clearly separate:

- confirmed facts,
- assumptions,
- information gaps,
- recommendations.
```

This is especially important when the output influences:

- project status,
- scope,
- budget,
- contracts,
- delivery commitments,
- executive reporting,
- risk acceptance.

---

# 9. Ask for Root Cause, Not Only Symptoms

A useful project-management analysis should go beyond the visible problem.

Instead of:

```text
The release is delayed.
```

Ask for:

```text
For each delivery issue, identify:

- symptom,
- likely root cause,
- affected dependency,
- project impact,
- corrective action,
- owner,
- escalation trigger.
```

This shifts the output from reporting to management analysis.

---

# 10. Make Recommendations Actionable

Avoid recommendations such as:

```text
Monitor the situation closely.
```

Prefer:

```text
Agree a recovery plan with the external API provider within
two working days and assess whether testing can continue using
a controlled mock service.
```

A useful recommendation should contain, where relevant:

- action,
- owner,
- priority,
- due date,
- escalation threshold.

---

# 11. Define Decision Criteria

For important project decisions, define the criteria before asking for a recommendation.

### Example

```text
Assess release readiness against:

- no unresolved Severity 1 defects,
- critical business processes tested,
- security approval received,
- rollback plan tested,
- support model operational,
- business owner approval received.
```

This makes the analysis more transparent and repeatable.

---

# 12. Define Escalation Triggers

Where possible, specify when an issue becomes a governance concern.

Examples:

```text
Escalate when:

- milestone delay exceeds 10 working days,
- budget variance exceeds the agreed tolerance,
- a critical dependency has no recovery plan,
- a critical defect remains unresolved close to release,
- a vendor misses a contractual commitment.
```

Escalation thresholds convert analysis into governance.

---

# 13. Match the Detail to the Audience

Different stakeholders require different information.

## Delivery Team

Focus on:

- blockers,
- actions,
- dependencies,
- ownership,
- deadlines.

## Steering Committee

Focus on:

- status,
- major risks,
- budget,
- schedule,
- decisions,
- escalations.

## Executive Sponsor

Focus on:

- business impact,
- strategic risk,
- major decisions,
- value,
- governance.

### Principle

Do not send the same level of detail to every audience.

---

# 14. Use AI for Decision Support, Not Automatic Decisions

Avoid:

```text
Decide whether we should go live.
```

Prefer:

```text
Assess go-live readiness against the defined criteria.

Identify blockers, manageable risks, assumptions, and unresolved
decisions.

Provide a recommendation with rationale.

The final decision remains with the accountable project stakeholders.
```

---

# 15. Build Quality Review Into the Prompt

Important prompts should include a review instruction.

### Example

```text
Before finalising:

- check for contradictions,
- identify unsupported assumptions,
- flag missing information,
- verify that recommendations are actionable,
- verify that ownership is clear,
- identify conclusions requiring independent validation.
```

This adds a second level of quality control.

---

# 16. Avoid False Precision

AI can produce precise-looking numbers that are unsupported by the available evidence.

Avoid:

```text
What is the exact probability this project will fail?
```

Prefer:

```text
Rate probability using the agreed project scale.

Explain the reasoning.

Identify what evidence would be required for a stronger assessment.
```

---

# 17. Protect Confidential Information

Do not include sensitive project information in public AI tools unless organisational policy explicitly allows it.

Remove or anonymise:

- client names,
- customer data,
- employee personal data,
- passwords,
- credentials,
- API keys,
- confidential pricing,
- protected contract information,
- proprietary financial data,
- security-sensitive architecture.

Use neutral placeholders where appropriate.

Examples:

```text
Client A
Vendor B
Project X
External API provider
Critical production platform
```

---

# 18. Keep Prompt Logic and Project Data Separate

Where possible, maintain:

```text
Reusable Prompt
+
Project-Specific Context
```

rather than embedding real project information inside the reusable prompt.

This improves:

- confidentiality,
- reuse,
- version control,
- maintenance,
- testing.

---

# 19. Design Prompts for Reuse

Use placeholders such as:

```text
[PROJECT]
[PHASE]
[DELIVERY APPROACH]
[KEY MILESTONE]
[KNOWN ISSUE]
[DEPENDENCY]
[STAKEHOLDER]
[METRIC]
```

A strong library prompt should work across multiple projects with minimal modification.

---

# 20. Align With Relevant Professional Practices

Individual prompts may reference relevant standards or delivery practices.

Examples:

- PMI / PMP
- PMBOK
- Agile
- Scrum
- Kanban
- hybrid delivery
- software testing
- DevOps
- risk management
- governance

Only include a standard or framework where it actually contributes to the task.

Do not use labels simply to make the prompt appear more sophisticated.

---

# 21. Treat Prompts as Managed Project Assets

A mature prompt should have:

- defined purpose,
- owner,
- version,
- review status,
- intended user,
- expected output,
- quality criteria,
- relevant framework alignment,
- review date.

Suggested lifecycle:

```text
Draft
↓
Tested
↓
Reviewed
↓
Approved
↓
Updated
↓
Retired
```

---

# Prompt Quality Checklist

Before adding a prompt to this repository, confirm:

- [ ] The business problem is clear
- [ ] The professional role is relevant
- [ ] There is one clear primary task
- [ ] The task is specific
- [ ] Sufficient context is provided
- [ ] The delivery framework is reflected where relevant
- [ ] The expected output is defined
- [ ] Facts and assumptions are separated
- [ ] Recommendations are actionable
- [ ] Ownership is visible
- [ ] Decision criteria are defined where needed
- [ ] Escalation criteria are defined where useful
- [ ] Human review is required
- [ ] Confidential information is protected
- [ ] The prompt can be reused
- [ ] Framework or standard references are relevant rather than decorative

---

# Key Principle

A high-quality project-management prompt is not defined by how long or sophisticated it sounds.

It is defined by whether it produces an output that is:

**relevant → structured → evidence-based → actionable → reviewable → governable.**
