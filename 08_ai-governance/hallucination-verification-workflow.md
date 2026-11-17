# Hallucination Verification Workflow

## Purpose

Use this workflow when AI produces information that sounds precise, authoritative, or highly confident.

Typical high-risk examples include:

- contract clauses,
- legal wording,
- technical specifications,
- financial calculations,
- standards,
- policies,
- dates,
- regulatory requirements.

The key principle is simple:

```text id="hallucination-core"
Confident Output
≠
Verified Fact
```

---

# Two-Step Verification Pattern

## Step 1 — Ask the Question

Example:

```text id="hallucination-step1"
What contract clause governs the notification period for a claim?

Provide the clause number and exact wording.
```

AI may return a very confident answer.

Do not stop there.

---

## Step 2 — Challenge the Answer

```text id="hallucination-step2"
How confident are you that the clause number and wording are
completely accurate?

What is the risk of error?

What source should I verify before using this in a formal document?
```

The purpose is to expose uncertainty before the information is used.

---

# Verification Workflow

Use:

```text id="hallucination-flow"
AI Answer
↓
Confidence Challenge
↓
Source Verification
↓
Human Review
↓
Approved Use
```

---

# What Requires Independent Verification

Always verify high-impact information such as:

```text id="hallucination-verify"
Contract clauses

Legal requirements

Financial figures

Technical specifications

Security recommendations

Standards

Regulatory requirements

Deadlines

Calculations
```

---

# Example — Contract Reference

AI says:

```text id="hallucination-contract"
Clause 12.4 requires notification within 10 days.
```

Before using it:

```text id="hallucination-contract-check"
Open the actual contract.

Verify the clause number.

Verify the wording.

Check related clauses.

Confirm with Commercial / Legal if material.
```

---

# Example — Technical Claim

AI says:

```text id="hallucination-tech"
This API supports 10,000 requests per second.
```

Verify using:

- vendor documentation,
- test evidence,
- architecture records,
- actual performance data.

---

# Example — Financial Calculation

AI says:

```text id="hallucination-finance"
The project variance is 7.4%.
```

Verify:

```text id="hallucination-finance-check"
Actual Cost

Approved Budget

Calculation

Reporting Period
```

---

# Fact / Assumption / Recommendation

Use this classification:

```text id="hallucination-classification"
FACT
Verified against an authoritative source.

ASSUMPTION
Used because information is missing.

AI ANALYSIS
Interpretation based on provided information.

RECOMMENDATION
Suggested future action.
```

Do not allow assumptions or AI analysis to become project facts automatically.

---

# Prompt — Verification Review

```text id="hallucination-review"
ROLE

You are a PMO quality reviewer.

TASK

Review the AI-generated content below.

[PASTE OUTPUT]

Identify statements that require independent verification.

For each provide:

Statement
Risk if Incorrect
Source to Verify
Priority

Do not assume the original AI answer is correct.
```

---

# Source Hierarchy

Prefer authoritative sources.

Example:

```text id="hallucination-source-hierarchy"
Original Contract
over
AI Summary

Official Product Documentation
over
AI Technical Claim

Approved Budget
over
AI Calculation

Project Schedule
over
AI Timeline Assumption
```

---

# High-Risk Warning Signs

Be especially cautious when AI provides:

```text id="hallucination-warning-signs"
Exact clause numbers

Exact quotations

Precise percentages

Specific deadlines

Legal conclusions

Security assurances

Guaranteed outcomes

Specific regulatory requirements
```

Precision can create a false sense of confidence.

---

# Do Not Ask AI to Verify Itself

Weak approach:

```text id="hallucination-self-check"
Are you sure?
```

Better:

```text id="hallucination-independent"
What authoritative source should I check?

What part of your answer is most likely to be wrong?

Which assumptions did you make?
```

The final verification should come from a real source, not just another AI response.

---

# Quality Checklist

Before using a high-impact AI answer:

- [ ] Source identified
- [ ] Original source checked
- [ ] Exact wording verified where relevant
- [ ] Numbers recalculated
- [ ] Dates checked
- [ ] Assumptions identified
- [ ] Related requirements reviewed
- [ ] Specialist review completed where required
- [ ] AI confidence not treated as proof

---

# Key Principle

Responsible use is:

```text id="hallucination-key"
Ask
↓
Challenge
↓
Verify
↓
Use
```

Not:

```text id="hallucination-bad"
Ask
↓
Trust
↓
Send
```

AI is a powerful drafting and analysis tool.

It is **not automatically an authoritative source**.

---

# Prompt Metadata

```text id="hallucination-metadata"
Prompt ID: AIGOV-002
Category: AI Governance
Version: 1.0
Status: Draft
Owner: Project Manager / PMO
Reviewer: Relevant Specialist
Risk Level: High
```

---

# Version History

| Version | Change |
|---|---|
| 1.0 | Initial hallucination verification workflow |
