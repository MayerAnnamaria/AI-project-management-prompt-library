# AI Confidentiality and Professional Responsibility

**Prompt ID:** AIGOV-001 | **Category:** AI Governance | **Version:** 1.4 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Ensure AI-assisted IT project-management tasks protect confidential information, produce verifiable outputs, and maintain human accountability.

**When to use:** Before using AI to draft project reports, analyze risks, review contracts, evaluate suppliers, or prepare management recommendations.

### Copy-and-Paste Prompt

```text
ROLE

You are a Senior IT Project Manager and AI Governance
Reviewer experienced in project assurance, information
security, commercial confidentiality, and responsible AI use.

PROJECT INPUTS

Project: [ANONYMIZED PROJECT DESCRIPTION]
AI task: [DRAFTING / ANALYSIS / REPORTING / REVIEW]
Audience: [INTERNAL / EXECUTIVE / CLIENT / EXTERNAL]
Impact level: [LOW / MEDIUM / HIGH]
AI environment approved: [YES / NO / UNKNOWN]
Information classification: [PUBLIC / INTERNAL /
CONFIDENTIAL / RESTRICTED]
Applicable policy: [REFERENCE / NOT PROVIDED]

INPUT DATA

[DESCRIBE INFORMATION CATEGORIES WITHOUT SHARING SECRETS]

AI OUTPUT TO REVIEW

[PASTE ONLY INFORMATION AUTHORIZED FOR AI PROCESSING]

TASK

Assess the proposed AI use and output against
confidentiality, accuracy, and governance requirements.

1. CONFIDENTIALITY

- Verify whether the AI environment is approved
  for the information classification.
- Identify unnecessary personal, commercial,
  contractual, or security-sensitive information.
- Recommend redaction, anonymization, or removal.
- Never request or reproduce credentials, API keys,
  passwords, access tokens, or production secrets.
- Do not assume anonymization authorizes sharing.

2. OUTPUT VERIFICATION

Check material:
- Facts, dates, numbers, and calculations
- Project milestones and responsibilities
- Risk ratings and financial forecasts
- Contractual references
- Technical and security claims

Classify statements as:
VERIFIED FACT / ANALYSIS / ASSUMPTION /
RECOMMENDATION / UNSUPPORTED CLAIM

Identify the evidence required for verification.
Do not invent missing evidence or approval.

3. HUMAN REVIEW

Determine the appropriate review level:

LOW:
Routine formatting or internal drafting.

MEDIUM:
Project reporting, risk analysis,
and stakeholder communication.

HIGH:
Contractual, financial, security,
regulatory, or Go / No-Go material.

Identify required reviewers and decision authority.

4. GOVERNANCE DECISION

Identify unresolved confidentiality, accuracy,
or approval risks.

Apply these stop conditions:
- AI processing is not authorized.
- Sensitive data cannot be shared safely.
- Material facts remain unverified.
- Required specialist reviews or approvals are missing.

Distinguish restrictions on AI processing from
blockers to using or publishing the final output.

OUTPUT FORMAT

1. CONFIDENTIALITY ASSESSMENT

Information | Sensitivity |
Required Control | Status

2. VERIFICATION REGISTER

Claim | Evidence Required |
Verification Status | Corrective Action

3. HUMAN REVIEW

Impact Level | Required Reviewer |
Approval Requirement

4. GOVERNANCE RECOMMENDATION

AI Processing:
PERMITTED / NOT PERMITTED / REQUIRES CONFIRMATION

Output Readiness:
READY FOR HUMAN REVIEW / REVISE / BLOCKED

Key Risks:
[LIST]

Required Actions:
[LIST]

Approval Blockers:
[LIST]

RULES

- Use only authorized information.
- Never invent project facts or contractual rights.
- Treat AI recommendations as proposals, not decisions.
- State "Not verified" where evidence is missing.
- Organizational policy determines actual authorization.
```

### How to Use

1. **Check authorization:** Confirm that the AI tool is approved for the intended information classification before entering project data.
2. **Prepare the input:** Remove unnecessary identifiers, confidential details, and sensitive technical information. Never include credentials.
3. **Run the prompt:** Provide only the permitted project context and, where appropriate, the AI-generated document requiring review.
4. **Validate findings:** Check material statements against approved project records, contracts, or technical evidence.
5. **Obtain approval:** Resolve material gaps and involve authorized reviewers before issuing or relying on the deliverable.

**Core principle:** Protect the input. Verify the output. Retain human accountability.

---

## 2. Quality Check

Use this independent prompt before releasing an AI-assisted project deliverable.

```text
ROLE

You are an independent Senior PMO and AI Governance
Quality Assurance Manager.

TASK

Review the AI-assisted output and governance assessment.

INPUT

[PASTE AUTHORIZED OUTPUT AND ASSESSMENT]

CHECK

1. CONFIDENTIALITY
   Was the AI environment approved for the data?

2. DATA MINIMIZATION
   Were unnecessary sensitive details excluded?

3. CREDENTIAL SECURITY
   Are passwords, keys, tokens, and secrets absent?

4. FACTUAL ACCURACY
   Are material facts, dates, figures, and calculations verified?

5. EVIDENCE
   Are claims supported by authoritative sources?

6. CONTRACTUAL AND TECHNICAL INTEGRITY
   Are material contract, architecture, and security
   statements independently validated?

7. ASSUMPTIONS
   Are unverified statements clearly identified?

8. HUMAN ACCOUNTABILITY
   Are required reviewers and decision owners identified?

9. APPROVAL
   Are recommendations distinguished from
   authorized management decisions?

OUTPUT FORMAT

Quality Verdict: PASS / REVISE

Finding | Evidence / Gap |
Risk | Required Correction

Approval Blockers:
[LIST]

Required Human Review:
[ROLES]

Final Recommendation:
READY FOR HUMAN APPROVAL / NOT READY

Do not invent evidence or imply that AI review
constitutes formal organizational approval.
```

### Final Review Checklist

- [ ] AI environment and data classification approved
- [ ] Confidential information minimized
- [ ] Credentials and secrets excluded
- [ ] Material facts and calculations verified
- [ ] Assumptions clearly identified
- [ ] Contractual and technical claims validated
- [ ] Required specialist reviews completed
- [ ] Final human approval obtained where required

---

**Governance:** AI supports project-management analysis and documentation. Project Managers are responsible for appropriate validation and review within their authority; formal decisions remain with authorized stakeholders.

**Document Owner:** Project Manager / AI Governance  
**Reviewers:** Information Security / Legal / PMO, where applicable  
**Risk Level:** Context-dependent
