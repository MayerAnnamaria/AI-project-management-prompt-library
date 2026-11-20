# Project AI Use Policy

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** AIGOV-003 | **Category:** AI Governance

---


## 1. Ready-to-Use Prompt

**Purpose:** Establish clear rules for the authorized, secure, and accountable use of generative AI in IT project delivery.

**When to use:** At project initiation, during team onboarding, or before introducing AI into project reporting, documentation, analysis, or stakeholder communication.

### Copy-and-Paste Prompt

```text
ROLE

You are a Senior IT Project Manager and AI Governance
Specialist experienced in information security,
project assurance, and responsible AI adoption.

PROJECT INPUTS

Project: [PROJECT NAME / ANONYMIZED DESCRIPTION]
AI tools approved: [LIST / NOT CONFIRMED]
Permitted AI activities: [LIST / NOT DEFINED]
Data classification rules: [POLICY REFERENCE]
Restricted information: [DATA CATEGORIES]
Required reviewers: [ROLES]
Approval authority: [ROLE / NOT CONFIRMED]
Applicable organizational policies: [REFERENCES]
Languages used: [IF RELEVANT]

TASK

Create or review a practical Project AI Use Policy
aligned with the provided organizational requirements.

1. APPROVED USE

Identify permitted activities, such as:
- Drafting non-sensitive documents
- Summarizing approved information
- Structuring meeting notes
- Brainstorming risks and options
- Improving wording and readability
- Reviewing documents for gaps
- Preparing draft reports and communications

Distinguish approved uses from proposed uses.

2. CONFIDENTIALITY AND RESTRICTIONS

- Require an approved AI environment.
- Identify restricted personal, commercial,
  contractual, and security-related information.
- Prohibit sharing credentials, passwords,
  API keys, tokens, and production secrets.
- Apply data minimization and appropriate redaction.
- Do not assume anonymization authorizes disclosure.

3. HUMAN REVIEW AND QUALITY

Require verification of:
- Facts, dates, and calculations
- Project milestones and responsibilities
- Technical and contractual claims
- Assumptions and recommendations
- Consistency with approved project records

4. APPROVAL AND ACCOUNTABILITY

- Define who may use AI for project work.
- Identify required reviewers and decision owners.
- Require specialist review for high-impact outputs.
- Keep formal approvals within project governance.
- Do not allow AI to authorize contractual,
  financial, security, or release decisions.

5. LANGUAGE AND TRANSLATION

- Allow AI-assisted translation where authorized.
- Require review of material translations.
- Verify technical terminology, deadlines,
  responsibilities, and contractual wording.
- Maintain consistency across language versions.

6. POLICY CONTROLS

Identify:
- Unapproved AI tools or use cases
- Restricted or incorrectly shared information
- Missing validation evidence
- Unclear reviewer or approval authority
- Required escalation or corrective actions

RULES

- Do not invent organizational permissions.
- Do not claim a tool is approved without evidence.
- Do not override existing security or privacy policies.
- Do not treat AI-generated content as verified fact.
- Do not imply AI review constitutes formal approval.
- Mark missing requirements as "To be confirmed".

OUTPUT FORMAT

1. PROJECT AI USE POLICY

Policy Area | Rule | Responsible Role

Include:
- Permitted AI uses
- Restricted information
- Human verification
- Specialist review
- Translation controls
- Decision authority

2. GOVERNANCE GAPS

Gap | Risk | Required Action | Proposed Owner

3. IMPLEMENTATION CHECKLIST

Control | Verification Required | Status

4. MANAGEMENT RECOMMENDATION

Policy Readiness:
READY FOR HUMAN REVIEW / REVISE / BLOCKED

Required Approvals:
[ROLES]

Outstanding Decisions:
[LIST]
```

### How to Use

1. **Confirm requirements:** Identify approved AI tools, permitted data classifications, and existing organizational policies.
2. **Complete the prompt:** Enter project-level rules and responsibilities without disclosing restricted information.
3. **Generate the policy:** Review the proposed rules, exceptions, and governance gaps.
4. **Validate:** Obtain relevant Information Security, Privacy, Legal, or PMO review.
5. **Approve and communicate:** Publish only the authorized policy and explain the applicable requirements to project team members.

**Important:** An AI-generated policy is a draft. It does not itself authorize the use of AI tools or the processing of confidential information.

---

## 2. Quality Check

Use this independent prompt before approving or distributing the Project AI Use Policy.

```text
ROLE

You are an independent Senior PMO and AI Governance
Quality Assurance Manager.

TASK

Review the proposed Project AI Use Policy against
the supplied organizational requirements.

INPUT

[PASTE POLICY AND APPROVED REQUIREMENTS]

CHECK

1. APPROVED USE
   Are permitted tools, activities, and users clear?

2. CONFIDENTIALITY
   Are data restrictions and minimization rules explicit?

3. CREDENTIAL SECURITY
   Are passwords, keys, tokens, and secrets prohibited?

4. ACCURACY
   Does the policy require factual verification
   of AI-generated project content?

5. HUMAN OVERSIGHT
   Are review responsibilities clearly assigned?

6. DECISION AUTHORITY
   Are formal approvals reserved for
   authorized stakeholders?

7. HIGH-IMPACT USE
   Are contractual, financial, security,
   and release-related outputs subject
   to appropriate specialist review?

8. TRANSLATION
   Are material multilingual communications
   subject to verification?

9. POLICY CONSISTENCY
   Does the document align with supplied
   organizational security and governance policies?

10. PRACTICAL USABILITY
    Can project team members understand
    what is allowed, prohibited, and required?

OUTPUT FORMAT

Quality Verdict: PASS / REVISE

Finding | Evidence / Gap |
Risk | Required Correction | Priority

Approval Blockers:
[LIST]

Required Human Review:
[ROLES]

Final Recommendation:
READY FOR HUMAN APPROVAL / NOT READY

Do not invent permissions, policy requirements,
review evidence, or organizational approvals.
```

### Final Quality Checklist

- [ ] Approved AI tools and permitted uses defined
- [ ] Data classification and confidentiality rules included
- [ ] Credentials and secrets prohibited
- [ ] Output verification requirements established
- [ ] Specialist review defined for high-impact outputs
- [ ] Human decision and approval authority clear
- [ ] Translation controls included where relevant
- [ ] Policy aligned with organizational requirements
- [ ] Relevant stakeholders have approved the policy

---

**Governance Principle:** AI may support project drafting, analysis, communication, and document review. Project teams remain responsible for appropriate use and validation, while formal decisions and approvals remain with authorized stakeholders.

**Document Owner:** Project Manager / AI Governance  
**Reviewers:** PMO / Information Security / Legal, as applicable  
**Risk Level:** Context-dependent

### Version History

| Version | Change |
|---|---|
| 1.0 | Initial Project AI Use Policy |
| 1.1 | Reorganized into a reusable policy prompt, usage instructions, and independent quality check |
