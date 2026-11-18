# AI Confidentiality and Professional Responsibility

**Prompt ID:** AIGOV-001 | **Category:** AI Governance | **Version:** 1.1 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Ensure AI-assisted project-management activities protect confidential information, preserve factual accuracy, and maintain human accountability.

**Use case:** Apply confidentiality and verification controls before using AI to draft, analyze, review, or communicate project information.

**Core principle: Protect the input. Verify the output.**

### Reusable AI Governance Prompt

Copy the prompt and replace the placeholders before using AI-generated material in a project workflow.

```text
ROLE

You are a Senior IT Project Manager and AI Governance Reviewer
experienced in information security, project assurance,
commercial confidentiality, and responsible AI use.

CONTEXT

Project type: [PROJECT TYPE]
AI task: [DRAFTING / ANALYSIS / REPORTING / REVIEW]
Intended audience: [INTERNAL / CLIENT / EXECUTIVE / EXTERNAL]
Business impact: [LOW / MEDIUM / HIGH]
Approved AI environment: [CONFIRMED / NOT CONFIRMED]
Applicable organizational AI policy: [POLICY / NOT PROVIDED]

INPUT CLASSIFICATION

Information to be processed:
[DESCRIBE DATA CATEGORIES WITHOUT DISCLOSING SECRETS]

Known restrictions:
[CONFIDENTIALITY / CONTRACTUAL / PRIVACY / SECURITY]

OUTPUT FOR REVIEW

[PASTE AN ANONYMIZED DRAFT IF SHARING IS PERMITTED]

TASK

Evaluate whether the proposed AI use and output
meet professional project-management standards.

STEP 1 — CONFIDENTIALITY AND DATA MINIMIZATION

1. Determine whether the AI environment is approved
   for the intended information classification.
2. Identify confidential or restricted information,
   including:
   - Personal or customer data
   - Client and project identifiers
   - Contract values and supplier rates
   - NDA-protected or commercially sensitive information
   - Security vulnerabilities and architecture details
   - Credentials, API keys, tokens, or production secrets
3. Recommend anonymization, redaction, or exclusion.
4. Retain only information necessary for the task.
5. Identify any required Information Security,
   Privacy, or Legal approval.

STEP 2 — OUTPUT ACCURACY

6. Identify statements requiring verification:
   - Facts and dates
   - Financial amounts and calculations
   - Project milestones and owners
   - Risk ratings and forecasts
   - Contract clauses
   - Technical and security claims
7. Distinguish:
   - Verified facts
   - AI analysis
   - Assumptions
   - Unsupported claims
8. Flag information that cannot be validated
   using the provided evidence.

STEP 3 — RISK-BASED HUMAN REVIEW

9. Classify the output's business impact:
   LOW: Routine formatting or drafting
   MEDIUM: Project reporting, risk analysis,
           stakeholder communications
   HIGH: Contractual, financial, security,
         regulatory, or Go / No-Go decisions

10. Recommend appropriate specialist review:
    - Project Manager / PMO
    - Business Owner / Finance
    - Information Security
    - Legal / Compliance
    - Technical Lead

STEP 4 — PROFESSIONAL ACCOUNTABILITY

11. Identify recommendations requiring formal approval.
12. Separate AI-assisted analysis from authorized decisions.
13. Confirm that the output is ready for human review,
    not automatically approved for distribution.

RULES

- Never request or reproduce passwords, API keys,
  access tokens, private keys, or production credentials.
- Do not process restricted information in an
  unapproved AI environment.
- Do not invent evidence, clauses, figures, or approvals.
- Do not treat AI recommendations as authorized decisions.
- If confidentiality cannot be established,
  recommend an approved alternative workflow.

OUTPUT FORMAT

1. CONFIDENTIALITY ASSESSMENT

Information Category | Sensitivity |
Potential Exposure | Required Control

2. DATA MINIMIZATION

Information to Retain |
Information to Remove / Anonymize |
Reason

3. OUTPUT VERIFICATION

Claim / Item | Evidence |
Verification Status | Required Action

4. RISK-BASED REVIEW

Output Type | Impact Level |
Required Reviewer | Approval Requirement

5. GOVERNANCE DECISION

Ready for Approved AI Processing:
YES / NO / REQUIRES CONFIRMATION

Output Ready for Human Approval:
YES / NO / REQUIRES REVISION

6. MANAGEMENT SUMMARY

- Main confidentiality concerns
- Unverified statements
- Required specialist reviews
- Approval blockers
- Recommended next action

Do not treat this assessment as permission to process data.
Actual permission must come from organizational policy.
```

### Essential Governance Rules

| Principle | Management Requirement |
|---|---|
| Confidentiality | Use only approved AI environments and permitted information |
| Data minimization | Share the minimum information necessary |
| Credential protection | Never include passwords, API keys, or production secrets |
| Accuracy | Verify material facts against approved sources |
| Contractual integrity | Check clause references against the actual agreement |
| Technical assurance | Validate security, architecture, and migration claims |
| Accountability | Keep decisions and approvals with authorized stakeholders |
| Traceability | Record evidence, reviewers, and approval status where required |

**Anonymization example**

Instead of:

```text
Client: ABC Bank
Vendor: XYZ Technologies
Contract Value: €4.2M
```

Use:

```text
Client: Financial-services organization
Vendor: External technology supplier
Project: Enterprise software implementation
```

Anonymization reduces disclosure risk but does not automatically make information safe to share. Commercial context, unique project details, or combinations of attributes may still identify a project.

---

## 2. Quality Check

Use this independent review before distributing or relying on AI-assisted project-management material.

```text
QUALITY CHECK

Act as an independent Senior PMO and AI Governance Reviewer.

Review the proposed AI-assisted task and output
against the supplied organizational requirements.

VERIFY

1. Confidentiality:
   Only permitted information was used.

2. Data Minimization:
   Unnecessary identifiers, commercial details,
   and sensitive technical information were excluded.

3. Credentials:
   No passwords, API keys, tokens, or secrets
   are included.

4. Factual Accuracy:
   Dates, figures, calculations, milestones,
   owners, and risk ratings are verified.

5. Evidence:
   Material conclusions are traceable
   to approved sources.

6. Contractual Accuracy:
   Clause references and obligations are checked
   against the original contract.

7. Technical Assurance:
   Architecture, security, and migration claims
   have appropriate validation evidence.

8. Human Oversight:
   Specialist review is proportionate
   to business and project impact.

9. Approval Authority:
   AI recommendations are not presented
   as authorized management decisions.

10. Distribution Readiness:
    The output contains no inappropriate disclosures
    or unsupported commitments.

OUTPUT

Quality Verdict: PASS / REVISE

Finding | Risk | Evidence |
Required Correction | Responsible Review Role

Approval Blockers:
[LIST]

Required Specialist Review:
[ROLES]

Final Assessment:
READY FOR HUMAN APPROVAL / NOT READY

A PASS verdict means the supplied material passed
this AI-assisted check. It does not replace formal
Information Security, Legal, PMO, or management approval.
```

---

## 3. Practical IT Use Case

### CRM Implementation — Confidential Risk Analysis

**Scenario:** A Project Manager is preparing a risk assessment for an enterprise CRM implementation. The source material contains client identifiers, contract values, supplier information, and an integration dependency.

The Project Manager wants to use AI to identify delivery risks without disclosing unnecessary commercial information or treating the resulting recommendations as approved project decisions.

### Project Context

| Attribute | Details |
|---|---|
| Project | Enterprise CRM Implementation |
| AI task | Delivery risk analysis |
| Project phase | Development / Integration |
| Supplier | External implementation partner |
| Main dependency | Identity-provider integration |
| Known concern | Certification delay affecting testing |
| Information sensitivity | Commercial and technical |
| AI environment approval | Not confirmed |
| Management objective | Assess risks while protecting confidential information |

### Example Input — Internal Source Information

<text color="secondary" size="xs">Fictional data used to demonstrate the transformation. Do not paste real restricted information into an unapproved tool.</text>

```text
Client:
ABC Bank

Supplier:
XYZ Technologies

Contract Value:
€4.2 million

Project:
Enterprise CRM Implementation

Current Issue:
Identity-provider certification is delayed.

Potential Impact:
System integration testing may be delayed.

Supplier Contract Reference:
Clause 14.3

Proposed Action:
Escalate to supplier management.
```

### Step 1 — Confidentiality Review

| Information | Sensitivity Concern | Recommended Action |
|---|---|---|
| Client identity | Confidential project identifier | Replace with industry description |
| Supplier name | Commercial relationship | Generalize |
| Contract value | Financial information | Remove if not required |
| Contract clause | Potentially confidential contractual detail | Remove unless needed and permitted |
| Certification dependency | Relevant technical context | Retain at an appropriate level |
| Testing impact | Essential for risk analysis | Retain |
| Proposed escalation | Management recommendation | Retain as proposed, not approved |

**Governance decision:** Do not submit the original information to an AI system until the organization's permitted-use requirements are confirmed.

### Step 2 — Minimized Project Context

If organizational policy permits the use of suitably generalized project information, the task could be reframed as:

```text
Project:
Enterprise software implementation
in the financial-services sector.

Delivery phase:
Integration testing preparation.

Dependency:
Certification of an external identity-provider integration.

Current concern:
Certification is delayed.

Potential impact:
System integration testing may start later
than planned.

Task:
Identify delivery risks, preventive actions,
escalation triggers, and information gaps.

Do not assume contractual penalties,
supplier responsibility, or an approved recovery plan.
```

This version retains the information needed to analyze the delivery dependency without unnecessarily exposing the client's identity, supplier identity, contract value, or clause reference.

### Step 3 — Example AI Risk Assessment

| Risk | Potential Impact | Proposed Mitigation | Verification Required |
|---|---|---|---|
| Certification delay | Integration testing may start late | Confirm supplier delivery forecast | Approved milestone and latest forecast |
| Testing compression | Reduced testing time | Assess resequencing opportunities | Test plan and coverage |
| Supplier dependency | Recovery options may be constrained | Establish escalation process | Supplier obligations and governance route |
| Release readiness | Downstream milestones may be affected | Conduct schedule impact assessment | Dependency and critical-path analysis |

These are possible delivery risks and proposed actions, not confirmed findings or authorized commitments.

### Step 4 — Output Verification

| AI Statement | Verification Requirement | Current Status |
|---|---|---|
| Certification is delayed | Supplier update and delivery baseline | Source-provided; evidence not independently verified |
| SIT may be delayed | Integrated project schedule | Assessment required |
| Testing can be re-sequenced | QA and Technical Lead assessment | Not confirmed |
| Supplier escalation is appropriate | Governance and contract review | Proposed |
| Contractual remedies exist | Original contract and Legal / Commercial review | Not established |

**Management conclusion:** The AI output can support a risk-review discussion but is not sufficient by itself to authorize supplier escalation or a change to the delivery baseline.

### Step 5 — Risk-Based Human Review

| Review Area | Responsible Role | Objective |
|---|---|---|
| Data confidentiality | Information Security / Privacy | Confirm appropriate AI-use controls |
| Risk accuracy | Project Manager | Validate the underlying dependency and impact |
| Schedule exposure | Project Planner / Delivery Lead | Confirm milestone implications |
| Technical feasibility | Solution Architect / QA Lead | Validate mitigation options |
| Commercial obligations | Commercial / Legal | Check contractual rights where relevant |
| Final decision | Authorized Project Stakeholder | Approve escalation or recovery action |

### Management Decisions

1. **Protect information:** Confirm approved AI usage and remove unnecessary sensitive details before processing.
2. **Validate risks:** Verify technical dependencies and schedule exposure against actual project evidence.
3. **Separate recommendations from authority:** Treat AI mitigation proposals as options requiring human review.
4. **Maintain traceability:** Record validated findings and authorized decisions in the project's normal governance records.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The example demonstrates effective data minimization and separates proposed risk responses from authorized decisions. However, AI environment approval and supporting delivery evidence have not been confirmed.

**Required corrections:**
- Verify that the intended AI environment is approved for the information classification.
- Confirm whether the generalized project context is permitted to be shared.
- Validate supplier dependencies and schedule implications.
- Review contractual issues against the actual agreement.
- Obtain appropriate human approval before implementing recommendations.

**Approval blockers:** Unconfirmed AI-use authorization and incomplete project evidence.

**Governance:** Supports responsible AI adoption, information security, project assurance, confidentiality, professional judgment, and accountable decision-making.

**Final principle:** AI can accelerate analysis and improve documentation, but responsibility for confidentiality, factual validation, and authorized decisions remains with the organization and its accountable professionals.
