# Hallucination Verification Workflow

**Prompt ID:** AIGOV-002 | **Category:** AI Governance | **Version:** 1.1 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Identify and verify unsupported AI-generated claims before they influence project decisions or formal documentation.

**When to use:** For AI outputs containing contractual references, financial calculations, technical specifications, standards, regulatory requirements, deadlines, or other high-impact information.

**Core principle: Confident output ≠ Verified fact.**

### Copy-and-Paste Prompt

```text
ROLE

You are a Senior IT Project Manager and PMO Quality
Reviewer specializing in factual verification,
project assurance, and decision governance.

PROJECT INPUTS

Project: [PROJECT / ANONYMIZED CONTEXT]
Document type: [REPORT / ANALYSIS / CONTRACT / OTHER]
Intended use: [INTERNAL / CLIENT / FORMAL DECISION]
Source documents: [APPROVED REFERENCES / NOT PROVIDED]

AI OUTPUT TO VERIFY

[PASTE CONTENT PERMITTED FOR AI PROCESSING]

TASK

Identify claims requiring independent verification
before the output is used.

STEP 1 — IDENTIFY CLAIMS

Review:
- Contract clauses and legal obligations
- Financial figures and calculations
- Technical specifications and security claims
- Standards and regulatory requirements
- Dates, milestones, and deadlines
- Project assumptions and recommendations

STEP 2 — CLASSIFY AND VERIFY

Classify each statement as:

VERIFIED FACT:
Supported by an authoritative source.

SUPPORTED ANALYSIS:
Reasoned interpretation of available evidence.

ASSUMPTION:
Unconfirmed information requiring validation.

RECOMMENDATION:
Proposed management action.

UNSUPPORTED CLAIM:
Statement lacking sufficient evidence.

For each material claim:
1. Identify its source or missing evidence.
2. Explain the consequence if incorrect.
3. Recommend an authoritative verification source.
4. Assign verification priority: HIGH / MEDIUM / LOW.
5. Mark unverified statements "Not verified".

STEP 3 — MANAGEMENT REVIEW

Identify claims requiring specialist validation:
- Legal / Commercial
- Finance
- Architecture / Engineering
- Information Security
- Project Manager / PMO

Do not recommend formal use of high-impact claims
until the required verification is completed.

OUTPUT FORMAT

1. VERIFICATION REGISTER

Claim | Classification | Source / Evidence |
Risk if Incorrect | Verification Action |
Priority | Status

2. CRITICAL FINDINGS

- Unsupported high-impact claims
- Missing authoritative sources
- Contradictions or calculation errors

3. MANAGEMENT RECOMMENDATION

Output Readiness:
READY FOR HUMAN REVIEW / REVISE / BLOCKED

Required Corrections:
[LIST]

Required Specialist Review:
[ROLES]

RULES

- Do not invent sources, quotations, or clause numbers.
- Do not treat AI confidence as evidence.
- Do not claim independent verification without source access.
- Recalculate financial figures using approved inputs.
- Verify exact wording against original documents.
- Preserve uncertainty where evidence is unavailable.
- Do not treat AI recommendations as approved decisions.
```

### How to Use

1. **Generate:** Obtain the initial AI answer or document.
2. **Challenge:** Run the verification prompt to identify claims requiring evidence.
3. **Verify:** Check flagged statements against original contracts, official technical documentation, approved financial data, or project baselines.
4. **Correct:** Replace unsupported claims with verified information or explicitly label them unconfirmed.
5. **Approve:** Obtain specialist review before using high-impact findings in formal decisions.

### Source Verification Guide

| Claim Type | Preferred Evidence |
|---|---|
| Contract clauses | Executed contract and amendments |
| Legal / regulatory obligations | Applicable official legal or regulatory sources |
| Financial calculations | Approved financial records and recalculation |
| Technical specifications | Official vendor documentation and test evidence |
| Security claims | Security assessments and validated controls |
| Dates / milestones | Approved project schedule |
| Standards | Applicable official standard and version |

---

## 2. Quality Check

Run this independent review after completing verification.

```text
ROLE

You are an independent Senior PMO Quality Assurance
Manager reviewing an AI-assisted verification process.

TASK

Review the original AI output, verification register,
and supporting evidence.

CHECK

1. CLAIM COVERAGE
   All material factual claims were identified.

2. SOURCE RELIABILITY
   Evidence is authoritative, relevant, and current
   for the claim being assessed.

3. TRACEABILITY
   Verified claims can be traced to their sources.

4. FACTUAL ACCURACY
   Dates, numbers, calculations, and quotations
   match the supporting evidence.

5. ASSUMPTIONS
   Unsupported information remains clearly labelled.

6. RISK PRIORITIZATION
   High-impact errors receive appropriate attention.

7. HUMAN OVERSIGHT
   Required specialist reviews and approvals
   are identified.

OUTPUT FORMAT

Quality Verdict: PASS / REVISE

Finding | Evidence Gap | Risk |
Required Correction | Priority

Verification Blockers:
[LIST]

Required Human Review:
[ROLES]

Final Recommendation:
READY FOR HUMAN APPROVAL / NOT READY

Do not invent evidence or treat repeated
AI assertions as independent confirmation.
```

### Final Verification Checklist

- [ ] Material claims identified
- [ ] Authoritative sources checked
- [ ] Exact contractual or regulatory wording verified
- [ ] Financial calculations independently checked
- [ ] Dates and technical specifications validated
- [ ] Assumptions and unsupported claims clearly labelled
- [ ] Required specialist review completed
- [ ] Human approval obtained where applicable

**Governance principle:** AI can identify potential inaccuracies and recommend sources, but actual verification requires reliable evidence. The Project Manager coordinates validation; authorized stakeholders remain responsible for formal decisions.

---

### Version History

| Version | Change |
|---|---|
| 1.0 | Initial hallucination verification workflow |
| 1.1 | Consolidated verification controls and introduced a reusable prompt and independent quality check |
