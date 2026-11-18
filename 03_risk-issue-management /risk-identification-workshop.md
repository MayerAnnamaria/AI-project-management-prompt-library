# Risk Identification Workshop

**Prompt ID:** RISK-002 | **Category:** Risk & Issue Management | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Facilitate structured, cross-functional risk identification to uncover project uncertainties, challenge assumptions, and strengthen the risk register.

**Use case:** Prepare and facilitate a risk workshop before software development, integration testing, major releases, or project re-planning when delivery teams must identify emerging risks and dependencies.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager and Risk Facilitator
specializing in software delivery, cross-functional risk
identification, workshop facilitation, and project governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target completion: [DATE]
Project team / workshop participants: [ROLES]
Systems and integrations: [LIST]
External vendors: [IF RELEVANT]
Known dependencies: [LIST]
Known assumptions: [LIST]
Known constraints: [LIST]
Known issues: [LIST]
Existing risks: [LIST / REGISTER]
Risk domains: [LIST / SELECT RELEVANT DOMAINS]
Workshop duration: [90 MINUTES / OTHER]
Workshop notes: [PASTE AFTER WORKSHOP, IF AVAILABLE]

TASK

Prepare and structure a cross-functional risk-identification workshop.

STEP 1 — WORKSHOP PREPARATION

1. Review project scope, milestones, architecture, assumptions,
   dependencies, existing risks, and known issues.
2. Select relevant risk domains, including where applicable:
   - Business / Product / Requirements
   - Architecture / Technology / Integration
   - Data / Security / Compliance
   - Infrastructure / Cloud
   - Testing / Quality / Release
   - Resources / Vendors / Schedule / Budget
   - Operations / Stakeholders / Governance
3. Generate 4–6 potential risks per selected domain.
4. Express each risk using cause–event–impact wording.
5. Provide 2–3 open-ended discussion questions per domain.
6. Identify workshop participants and preparation materials.
7. Treat AI-generated risks as discussion starters,
   not confirmed project risks.

STEP 2 — WORKSHOP FACILITATION

8. Create a 90-minute workshop agenda with activities,
   facilitation guidance, and expected participant outputs.
9. Challenge unverified assumptions and cross-team dependencies.
10. Encourage participants to identify additional risks
    beyond the AI-generated seed list.
11. Capture risks before debating mitigation solutions.
12. Distinguish uncertain future risks from existing issues.
13. Identify common causes, cascading effects, and
    dependencies affecting multiple workstreams.
14. Avoid premature scoring, ownership assignment,
    or dismissal of potential risks.

STEP 3 — WORKSHOP CONSOLIDATION

15. Structure workshop findings into clear risk statements.
16. Remove genuine duplicates without losing distinct
    causes, events, or potential impacts.
17. Separate confirmed workshop findings from AI suggestions
    that participants have not validated.
18. Identify missing evidence required for risk assessment.
19. Propose risk owners for stakeholder confirmation.
20. Identify cross-functional risks requiring joint review.
21. Recommend next steps for scoring, mitigation,
    escalation, and formal risk-register updates.

Do not invent project facts, risk evidence, or approvals.
Do not assign likelihood or impact scores during identification.
Do not present the AI seed list as a complete risk register.
Adapt workshop questions to the actual project and delivery approach.

OUTPUT FORMAT

1. WORKSHOP PREPARATION

Objective | Required Input | Participants |
Preparation Action | Owner

2. RISK IDENTIFICATION SEED LIST

For each selected domain provide:
- 4–6 potential risks
- 2–3 workshop questions

Risk ID | Domain | Potential Risk (Cause–Event–Impact) |
Affected Workstream | Discussion Focus

3. WORKSHOP AGENDA

Time | Activity | Purpose |
Facilitator Action | Participant Output

Default duration: 90 minutes.

4. CONSOLIDATED RISK CANDIDATES

Risk ID | Category | Risk Statement | Cause |
Potential Impact | Source / Workstream |
Proposed Owner | Evidence Required Before Scoring |
Validation Status

If workshop notes are unavailable, mark all generated
entries as unvalidated candidates.

5. CROSS-FUNCTIONAL RISK REVIEW

Risk / Dependency | Affected Areas |
Common Root Cause | Potential Cascading Impact |
Management Concern

6. FOLLOW-UP ACTIONS

Action | Priority | Proposed Owner |
Required By | Expected Outcome

7. MANAGEMENT SUMMARY

- Most significant potential risks and shared dependencies
- Assumptions requiring validation
- Current issues requiring separate management
- Risks requiring specialist or governance attention
- Recommended next steps for formal assessment

Use concise Markdown tables.
Mark unknown information as "Not yet defined".
Do not treat unvalidated candidates as approved risk records.
```

---

## 2. Quality Check

Apply this control after generating the workshop materials and, where available, consolidating the workshop notes.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the risk workshop outputs.

Verify:

1. Completeness: Relevant risk domains, workshop questions,
   agenda, consolidation, and follow-up actions are included.
2. Accuracy: AI-generated candidates are distinguished
   from participant-validated risks and actual issues.
3. Risk Quality: Statements identify credible causes,
   uncertain events, and potential consequences.
4. Coverage: Technical, business, security, vendor,
   operational, and cross-team risks are considered
   where relevant.
5. Facilitation: The agenda is realistic, encourages
   participant input, and avoids premature scoring.
6. Consolidation: Duplicates are reviewed without
   removing materially different risks.
7. Governance: Missing evidence, proposed owners,
   validation responsibilities, and next steps are visible.
8. Actionability: Findings can be transferred into
   a formal risk assessment process.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Validation Blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent participant agreement, risk ratings,
final ownership, or approval decisions.
Flag items requiring human validation.
```

---

## 3. Practical IT Use Case

### E-commerce Software Development — Payment Integration Risk Workshop

**Scenario:** An e-commerce team is developing a new checkout feature using an external payment gateway. Before integration testing, the Project Manager organizes a risk-identification workshop to uncover technical, security, testing, and supplier-related uncertainties that could threaten the release.

### Project Context

| Attribute | Details |
|---|---|
| Project | E-commerce Checkout Enhancement |
| Phase | Development / Pre-Integration Testing |
| Delivery approach | Scrum |
| Release target | 30 September 2027 |
| Team | Product Owner, Developers, QA Lead, Security Lead, Project Manager |
| External dependency | Payment Gateway Provider |
| Key systems | Web Application, Payment API, Order Management System |
| Known concern | Payment API integration and testing readiness |
| Management decision | Identify and validate potential delivery risks before SIT |

### Example Input

```text
Project: E-commerce Checkout Enhancement

Business objective:
Improve checkout functionality and introduce
a new external payment gateway.

Project phase: Development / Pre-Integration Testing
Delivery approach: Scrum
Target release: 30 September 2027

Project team:
- 1 Project Manager
- 1 Product Owner
- 4 Developers
- 2 QA Engineers
- 1 Security Lead

External vendor:
Payment Gateway Provider

Systems:
E-commerce Web Application
Payment Gateway API
Order Management System

Known dependencies:
- Payment API integration
- Test environment availability
- Security review
- Payment transaction validation
- Business acceptance testing

Known assumptions:
- Payment API documentation is complete.
- Test environment supports required payment scenarios.
- Payment-provider support will be available during SIT.

Known constraints:
- Fixed September release target
- Limited QA capacity

Known issue:
Payment-provider sandbox access has not yet been granted.

Workshop objective:
Identify potential integration, security, testing,
and release risks before SIT.
```

### Example Output — Risk Identification Workshop

#### 1. Workshop Preparation

| Objective | Required Input | Participants | Preparation Action | Proposed Owner |
|---|---|---|---|---|
| Identify integration risks | API specification, interface design | Developers, Vendor Lead | Review dependencies | Technical Lead |
| Identify testing risks | Test strategy, environments | QA Lead, Developers | Review test coverage | QA Lead |
| Identify security risks | Security requirements | Security Lead, Architect | Review security assumptions | Security Lead |
| Identify release risks | Roadmap, milestone plan | PM, Product Owner | Review delivery constraints | Project Manager |

Participants should review known assumptions, dependencies, and existing issues before the workshop.

#### 2. Risk Identification Seed List

The following risks are **AI-generated discussion candidates**, not validated project risks.

**Domain A — Integration**

| ID | Potential Risk | Discussion Focus |
|---|---|---|
| A-01 | If the payment API specification changes during development, integration rework may delay SIT. | API stability |
| A-02 | If payment-provider response behavior differs from documentation, transaction processing defects may delay testing. | Interface reliability |
| A-03 | If error-handling responsibilities are unclear, failed payments may not be processed consistently. | Technical ownership |
| A-04 | If payment gateway and order-management integration assumptions are incorrect, transaction reconciliation may require redesign. | Cross-system dependency |

**Workshop questions:**

- Which payment API assumptions remain unverified?
- What happens if the provider changes an interface during development?
- Who owns payment failures across the application and gateway?

**Domain B — Security and Compliance**

| ID | Potential Risk | Discussion Focus |
|---|---|---|
| B-01 | If payment data handling does not meet applicable security requirements, remediation may delay approval. | Data protection |
| B-02 | If security testing identifies critical vulnerabilities late, the release may be delayed. | Security readiness |
| B-03 | If access permissions are incorrectly configured, unauthorized transaction access could occur. | Authorization controls |
| B-04 | If supplier security evidence is unavailable when required, the security review may remain incomplete. | Vendor assurance |

**Workshop questions:**

- Which security requirements require formal approval?
- What sensitive data will pass through the integration?
- Which security controls depend on the payment provider?

**Domain C — Testing and Release**

| ID | Potential Risk | Discussion Focus |
|---|---|---|
| C-01 | If sandbox access remains unavailable, integration testing may start late. | Environment readiness |
| C-02 | If transaction test scenarios are incomplete, critical defects may escape into production. | Test coverage |
| C-03 | If QA capacity is insufficient, regression testing may not finish before release readiness. | Resource availability |
| C-04 | If payment exception scenarios remain untested, release approval may be blocked. | Acceptance criteria |

**Workshop questions:**

- Which payment scenarios are not yet covered by testing?
- How much schedule flexibility exists if SIT starts late?
- What evidence is required before payment functionality can be released?

#### 3. Workshop Agenda

<text></text>

| Time | Activity | Purpose | Facilitator Action | Participant Output |
|---|---|---|---|---|
| 0–10 min | Context and objectives | Align participants | Review scope and constraints | Shared understanding |
| 10–20 min | Existing risks and assumptions | Establish baseline | Challenge assumptions | Open questions |
| 20–55 min | Domain-based identification | Generate potential risks | Facilitate cross-functional discussion | Candidate risks |
| 55–70 min | Dependency review | Identify cascading exposure | Trace cross-team impacts | Dependency risks |
| 70–80 min | Consolidation | Review overlapping risks | Clarify causes and consequences | Refined statements |
| 80–90 min | Actions and next steps | Prepare formal assessment | Identify evidence and validation needs | Follow-up actions |

**Facilitation principle:** Capture and clarify risk statements before moving to mitigation or scoring.

#### 4. Consolidated Risk Candidates

No actual workshop notes have been provided. The following is an **illustrative consolidation**, not a record of completed participant decisions.

| Risk ID | Category | Risk Statement | Cause | Potential Impact | Proposed Owner | Evidence Required |
|---|---|---|---|---|---|---|
| R-01 | Integration | API changes may require integration rework and delay SIT | Unconfirmed API stability | Schedule / Cost | Technical Lead | Provider specification and change policy |
| R-02 | Testing | Continued sandbox unavailability may delay integration test execution | Access dependency | Schedule / Quality | QA Lead | Confirmed access date |
| R-03 | Security | Late identification of security gaps may delay release approval | Incomplete security validation | Security / Schedule | Security Lead | Security assessment |
| R-04 | Resources | Limited QA capacity may prevent completion of required regression tests | Competing resource demand | Schedule / Quality | QA Lead | Capacity forecast |
| R-05 | Integration | Unclear failure-handling ownership may result in inconsistent payment processing | Cross-system responsibility gap | Quality / Operations | Technical Lead | Interface responsibility agreement |

**Validation status:** All five entries are unvalidated workshop candidates.

The lack of sandbox access is a current **issue**. R-02 describes the uncertain future impact if it remains unresolved, rather than treating the access failure itself as a future risk.

#### 5. Cross-Functional Risk Review

| Risk / Dependency | Affected Areas | Common Root Cause | Potential Cascading Impact | Management Concern |
|---|---|---|---|---|
| Payment API readiness | Development, Integration, QA | External dependency | Integration delay → SIT delay → Release risk | Vendor readiness |
| Sandbox availability | Vendor, QA, Development | Missing environment access | Delayed testing → Compressed regression | Environment ownership |
| Security approval | Security, Development, Release | Unverified controls | Remediation → Retesting → Approval delay | Release readiness |
| QA capacity | QA, Product, Delivery | Shared resources | Reduced coverage → Defects → Acceptance risk | Delivery feasibility |

#### 6. Follow-Up Actions

| Action | Priority | Proposed Owner | Required By | Expected Outcome |
|---|---|---|---|---|
| Confirm payment sandbox access | High | Technical Lead / Vendor | Before SIT | Test environment readiness |
| Validate API documentation | High | Development Lead | Before integration completion | Reduced technical uncertainty |
| Review payment security requirements | High | Security Lead | Before security testing | Defined approval requirements |
| Confirm QA capacity and coverage | High | QA Lead | Before SIT planning approval | Feasible test plan |
| Validate and score candidate risks | High | Project Manager / Risk Owners | After workshop | Updated risk register |

### Management Decisions

1. **Integration readiness:** Confirm payment API and sandbox dependencies before committing to the SIT schedule.
2. **Quality assurance:** Validate available QA capacity and test coverage for critical payment scenarios.
3. **Security governance:** Agree on payment security and compliance requirements, assessment ownership, and approval evidence.
4. **Risk management:** Validate candidate risks with participants, then assign ownership and conduct qualitative assessment.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The workshop materials cover relevant technical, testing, security, and cross-functional risks. However, the risk candidates have not been validated by participants, supplier readiness remains unconfirmed, and the existing sandbox-access issue requires separate tracking.

**Required corrections:**
- Conduct the workshop with relevant technical and business stakeholders.
- Validate and refine the proposed risks.
- Confirm payment API and environment dependencies.
- Separate the sandbox-access issue from its potential schedule consequences.
- Assign confirmed risk owners and complete risk scoring after identification.

**Validation blockers:** Missing participant validation, unresolved environment access, and unconfirmed supplier readiness.

**Governance:** This framework supports PMI-aligned practices in risk identification, stakeholder engagement, facilitation, dependency management, and uncertainty management.

AI-generated risk candidates are preparation materials, not an approved risk register. Risk statements, ownership, prioritization, and responses require human validation. Protect confidential technical, payment, customer, vendor, and security-sensitive information.
