# Prompt Design Principles

This repository follows a consistent set of prompt-design principles to ensure that AI-supported project-management work is structured, reusable, and professionally reviewable.

The objective is not to make prompts unnecessarily complex.

The objective is to make them **clear enough to support real project decisions**.

---

# 1. Define a Relevant Professional Role

Avoid generic roles.

### Weak

```text
You are a project manager.
```

### Better

```text
You are a senior IT Project Manager experienced in software delivery,
stakeholder management, risk management, testing coordination,
and cross-functional project governance.
```

The role should match the task.

Examples:

- Risk Manager for risk analysis
- QA Manager for test readiness
- PMO Lead for governance review
- Business Analyst for requirement analysis
- Delivery Manager for execution issues

### Principle

Use the **most relevant expertise**, not the most senior-sounding title.

---

# 2. One Primary Task per Prompt

Avoid combining unrelated tasks.

### Weak

```text
Review the risks, create a status report, write an escalation email,
and prepare a stakeholder matrix.
```

### Better

Break the work into separate prompts:

1. Risk review
2. Status report
3. Escalation communication
4. Stakeholder analysis

This improves:

- output quality,
- reusability,
- reviewability,
- and version control.

---

# 3. Make the Ask Specific

Avoid vague requests.

### Weak

```text
Analyse this project.
```

### Better

```text
Identify the five delivery risks most likely to affect the planned
go-live date within the next eight weeks.
```

A strong task should define:

- what should be analysed,
- what time horizon matters,
- what decision it supports,
- and what output is expected.

---

# 4. Provide Relevant Context

AI output becomes more useful when it understands the project environment.

Useful context may include:

- project objective,
- current phase,
- delivery methodology,
- timeline,
- milestone status,
- team structure,
- external vendors,
- dependencies,
- known issues,
- key stakeholders,
- business constraints,
- technical constraints.

### Weak

```text
What risks do you see?
```

### Better

```text
The project is six weeks from UAT.

The external API provider is two weeks behind certification.

Data migration reconciliation is currently at 96%.

Two critical defects remain open.

Identify the risks that could delay UAT or go-live.
```

---

# 5. Define the Output Format

Do not leave the final structure to the AI.

### Example

```text
Provide a table with:

Risk
Root Cause
Probability
Impact
Mitigation
Owner
Due Date
```

Output formats may include:

- tables,
- executive summaries,
- bullet-point updates,
- action lists,
- decision logs,
- structured reports,
- escalation messages.

The format should match the intended audience.

---

# 6. Separate Facts from Assumptions

AI should not fill missing information silently.

Use:

```text
Do not invent missing project information.

Clearly separate:

- confirmed facts,
- assumptions,
- information gaps,
- recommendations.
```

This is particularly important when the output influences:

- project status,
- budget,
- risk decisions,
- scope,
- delivery commitments,
- executive reporting.

---

# 7. Ask for Root Cause, Not Only Symptoms

A useful project-management analysis should go beyond what is visible.

### Example

Instead of:

```text
The project is delayed.
```

Ask for:

```text
For each delay, identify:

- symptom,
- likely root cause,
- project impact,
- dependency impact,
- corrective action,
- owner.
```

This turns reporting into management analysis.

---

# 8. Make Recommendations Actionable

Avoid recommendations such as:

```text
Monitor the issue closely.
```

Prefer:

```text
Escalate the API certification delay to the vendor delivery manager,
agree a recovery plan within two working days, and assess whether
UAT can start using a controlled mock environment.
```

A useful recommendation should contain:

- action,
- owner,
- priority,
- due date,
- escalation threshold where relevant.

---

# 9. Include Decision Criteria

For important decisions, define the evaluation criteria explicitly.

### Example

```text
Assess go-live readiness against the following criteria:

- no Severity 1 defects,
- all critical business processes tested,
- data migration reconciliation above 99.5%,
- rollback plan tested,
- operational support team trained,
- business owner approval received.
```

This makes the analysis more transparent and repeatable.

---

# 10. Define Escalation Triggers

Where possible, specify when an issue must be escalated.

Examples:

```text
Escalate when:

- milestone delay exceeds 10 working days,
- budget variance exceeds 5%,
- a critical dependency has no agreed recovery plan,
- a Severity 1 defect remains open within five days of go-live.
```

Escalation thresholds help convert analysis into governance.

---

# 11. Match the Detail to the Audience

Different stakeholders need different levels of detail.

## Delivery Team

Focus on:

- actions,
- blockers,
- dependencies,
- owners,
- deadlines.

## Steering Committee

Focus on:

- overall status,
- major risks,
- budget,
- timeline,
- decisions required.

## Executive Sponsor

Focus on:

- business impact,
- strategic risk,
- decisions,
- escalation.

### Principle

Do not provide the same output to every stakeholder.

---

# 12. Use AI for Decision Support, Not Automatic Decisions

Avoid prompts such as:

```text
Decide whether we should go live.
```

Prefer:

```text
Assess go-live readiness against the defined criteria.

Identify blockers, risks, assumptions, and unresolved decisions.

Provide a recommendation with supporting rationale.

The final decision remains with the accountable project stakeholders.
```

---

# 13. Build Review into the Prompt

Every important prompt should include a review instruction.

Example:

```text
Before finalising the output:

- check for contradictions,
- identify unsupported assumptions,
- highlight missing information,
- verify that every recommendation has an owner,
- flag any conclusion that requires independent validation.
```

This creates a second layer of quality control.

---

# 14. Avoid False Precision

AI may produce precise numbers even when the input does not justify them.

Avoid asking:

```text
What is the exact probability this project will fail?
```

Prefer:

```text
Rate probability as Low / Medium / High based only on the information provided.

Explain the reasoning and identify any missing evidence.
```

---

# 15. Protect Confidential Information

Never include sensitive project information in a public AI tool unless your organisation explicitly permits it.

Anonymise where necessary.

### Do not include:

- client names,
- personal data,
- credentials,
- passwords,
- API keys,
- confidential pricing,
- confidential contract information,
- sensitive financial data,
- proprietary architecture,
- security information.

Use:

```text
Client A
Vendor B
€XM programme
External API provider
Critical business system
```

instead of identifiable information.

---

# 16. Design Prompts for Reuse

Avoid creating prompts that only work once.

Use placeholders such as:

```text
[PROJECT NAME]
[CURRENT PHASE]
[KEY MILESTONE]
[KNOWN ISSUE]
[DEPENDENCY]
[STAKEHOLDER]
```

A reusable prompt should work across different projects with minimal modification.

---

# 17. Keep Prompt and Project Data Separate

Where possible, maintain:

```text
Reusable Prompt
+
Project-Specific Context
```

rather than embedding real project details directly into the master prompt.

This makes:

- maintenance easier,
- versioning clearer,
- reuse safer,
- confidentiality easier to manage.

---

# 18. Review Prompts Like Project Assets

A mature prompt library should treat prompts as managed assets.

Each prompt should have:

- business purpose,
- owner,
- version,
- review status,
- last review date,
- intended audience,
- expected output,
- quality criteria.

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

- [ ] Is the professional role relevant?
- [ ] Is there one clear task?
- [ ] Is the task specific?
- [ ] Is sufficient context provided?
- [ ] Is the expected output defined?
- [ ] Are assumptions handled explicitly?
- [ ] Are recommendations actionable?
- [ ] Are owners included where relevant?
- [ ] Are escalation criteria defined where useful?
- [ ] Is human review required?
- [ ] Has confidential information been removed?
- [ ] Can the prompt be reused on another project?

---

# Key Principle

A high-quality prompt is not defined by how sophisticated it sounds.

It is defined by whether it produces an output that is:

**relevant, structured, reviewable, actionable, and safe to use in a professional project environment.**
