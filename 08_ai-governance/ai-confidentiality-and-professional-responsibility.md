# AI Confidentiality and Professional Responsibility

## Purpose

AI can support project managers with drafting, analysis, summarisation, and document review.

It does **not** remove responsibility for:

- confidentiality,
- accuracy,
- professional judgement,
- and final approval.

Two rules should guide every AI-assisted PM task:

```text
Protect the input.
Verify the output.
```

---

# 1. Protect Confidential Information

Before entering project information into an AI tool, confirm that the information is permitted to be shared with that system.

Avoid entering sensitive information such as:

- client or project identifiers,
- personal data,
- contract values and rates,
- confidential commercial information,
- bid or negotiation strategy,
- NDA-protected material,
- security vulnerabilities,
- production credentials,
- API keys or passwords,
- proprietary technical information.

Where possible, anonymise project data.

### Example

Instead of:

```text
Client: ABC Bank
Vendor: XYZ Technologies
Contract Value: €4.2M
```

use:

```text
Client: Financial-services organisation
Vendor: External technology supplier
Project: Enterprise software implementation
```

---

# Data-Minimisation Principle

Provide only the information required for the task.

```text
Necessary Context
≠
All Available Project Information
```

A risk analysis may require:

- the dependency,
- current delay,
- project impact,
- milestone.

It may not require:

- customer identity,
- commercial rates,
- contract numbers,
- internal emails.

---

# Credentials

Never include:

```text
Passwords
API keys
Access tokens
Private keys
Database credentials
Production secrets
```

Credentials are not project context.

---

# 2. Verify AI Output

AI-generated information should not automatically be treated as project fact.

Use:

```text
Approved Source
↓
Verified Fact
↓
AI Draft / Analysis
↓
Human Review
```

Not:

```text
AI Output
↓
Assumed Fact
```

---

# What Must Be Verified

Before issuing AI-assisted project material, verify:

- facts,
- dates,
- numbers,
- calculations,
- owners,
- milestones,
- risk ratings,
- contractual references,
- technical claims,
- assumptions.

---

# Contract References

Never rely on AI-generated clause numbers or contractual wording without checking the actual contract.

```text
AI Interpretation
↓
Original Contract
↓
Commercial / Legal Review where required
```

AI may support contract analysis.

It is not the final contractual authority.

---

# Technical Claims

Statements such as:

```text
"This configuration is secure."

"This architecture will scale."

"This migration will not lose data."
```

require evidence.

AI wording does not replace:

- technical validation,
- testing,
- architecture review,
- or security approval.

---

# AI Recommendations Are Not Decisions

AI may recommend:

- delaying a release,
- escalating a vendor,
- accepting a risk,
- changing scope,
- increasing resources.

The decision still belongs to the authorised stakeholder.

```text
AI
Supports Analysis

Project Manager
Validates and Recommends

Decision Owner
Approves
```

---

# Risk-Based Human Review

Use stronger review for higher-impact outputs.

### Lower Impact

Examples:

- formatting notes,
- structuring meeting minutes,
- rewriting internal text.

### Medium Impact

Examples:

- status reports,
- risk analysis,
- stakeholder communications.

### High Impact

Examples:

- contractual notices,
- financial forecasts,
- security recommendations,
- Go / No-Go papers,
- legal or regulatory material.

High-impact outputs should receive appropriate specialist review.

---

# Professional Responsibility Checklist

Before using an AI-assisted output:

- [ ] Full output reviewed
- [ ] Facts verified
- [ ] Dates verified
- [ ] Numbers verified
- [ ] Assumptions identified
- [ ] Contract references verified where relevant
- [ ] Technical claims checked
- [ ] Confidential information handled correctly
- [ ] Appropriate specialist review completed
- [ ] Final human approval obtained

---

# Governance Model

```text
Before AI
↓
Confidentiality Check

During AI
↓
Controlled Prompting

After AI
↓
Accuracy Review

Before Issue
↓
Human Approval
```

---

# Key Principle

Responsible AI use is not:

```text
Prompt
↓
Copy
↓
Send
```

It is:

```text
Protect
↓
Prompt
↓
Verify
↓
Review
↓
Approve
```

AI supports project-management decisions.

**The Project Manager remains accountable for the final output.**

---

# Prompt Metadata

```text
Prompt ID: AIGOV-001
Category: AI Governance
Version: 1.1
Status: Draft
Owner: Project Manager / AI Governance
Reviewer: Information Security / Legal / PMO where applicable
Risk Level: High
```

---

# Version History

| Version | Change |
|---|---|
| 1.0 | Initial governance framework |
| 1.1 | Simplified for concise GitHub playbook use |
