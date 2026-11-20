# Work Breakdown Structure

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** PLAN-001 | **Category:** Project Planning

---


## 1. Ready-to-Use Prompt

**Purpose:** Decompose approved project scope into manageable deliverables and work packages to support planning, estimating, ownership, and delivery control.

**Use case:** Develop or revise a deliverable-based WBS when preparing an IT project schedule, estimating resources and costs, allocating responsibilities, or assessing the impact of scope changes.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software delivery,
scope decomposition, work package planning, dependency management,
resource planning, and project governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project type: [SOFTWARE / DATA / INFRASTRUCTURE / ERP / OTHER]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Approved scope: [LIST / REFERENCE]
Key deliverables: [LIST]
Known workstreams: [LIST]
Systems and integrations: [LIST]
Dependencies: [LIST]
Vendors: [IF RELEVANT]
Milestones: [LIST]
Constraints: [LIST]
Available project roles: [LIST]

TASK

Create a deliverable-oriented, three-level Work Breakdown Structure
and review its planning completeness.

STEP 1 — WBS DEVELOPMENT

1. Decompose confirmed project scope into a three-level hierarchy.
2. Group work logically by major deliverables or delivery areas.
3. Use Level 1 for major deliverables or delivery areas,
   Level 2 for work packages, and Level 3 for sub-deliverables
   or planning-level work components.
4. Apply consistent hierarchical numbering (1.0, 1.1, 1.1.1).
5. Identify the primary owner, major dependency, and measurable
   completion criterion for each Level 2 work package.
6. Ensure deliverables are traceable to approved scope.
7. Include governance, requirements, design, development,
   integration, testing, security, deployment, transition,
   and close-out where relevant.
8. Include vendor deliverables and cross-team interfaces
   where supported by project information.

STEP 2 — COMPLETENESS AND SCHEDULE REVIEW

9. Identify missing or duplicated work packages.
10. Flag unclear boundaries, ownership, and dependencies.
11. Identify potentially required but unconfirmed work separately.
12. Check dependencies between workstreams and delivery milestones.
13. Identify work packages requiring detailed scheduling,
    cost estimation, or additional resource planning.
14. Highlight scope gaps, delivery risks, and governance decisions.
15. Recommend corrections before approving the WBS.

Do not invent scope, deliverables, owners, or commitments.
Distinguish approved work from proposed additions.
Avoid excessive task-level decomposition.
Do not confuse business outcomes with project deliverables.

Adapt the hierarchy to the delivery approach.
For Agile or Scrum, align relevant WBS elements with product
capabilities and releases without replacing the Product Backlog.
For Kanban, avoid imposing unnecessary task-level hierarchy.

OUTPUT FORMAT

1. THREE-LEVEL WORK BREAKDOWN STRUCTURE

Use an indented hierarchy:

1.0 [MAJOR DELIVERABLE / DELIVERY AREA]
    1.1 [WORK PACKAGE]
        1.1.1 [SUB-DELIVERABLE / WORK COMPONENT]

2. WORK PACKAGE REGISTER

WBS ID | Work Package | Primary Owner |
Major Dependency | Completion Criterion | Scope Status

3. WBS GAP REVIEW

Missing / Unclear Work | Potential Impact |
Recommended WBS Location | Proposed Action | Priority

4. CROSS-WORKSTREAM DEPENDENCIES

WBS ID | Dependency | Provider / Owner |
Receiving Work Package | Delivery Impact

5. WBS-TO-SCHEDULE MAPPING

WBS ID | Work Package | Detailed Scheduling Required? |
Key Dependency | Related Milestone

6. MANAGEMENT SUMMARY

- Major deliverables and scope coverage
- Missing or duplicated work
- Critical dependencies and ownership gaps
- Work packages requiring detailed planning
- Recommended corrections and approval decisions

Use concise Markdown tables.
Mark missing information as "Not yet defined".
Flag unapproved work packages separately from the WBS baseline.
```

---

## 2. Quality Check

Apply this control after generating the Work Breakdown Structure.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the Work Breakdown Structure.

Verify:

1. Completeness: All confirmed project deliverables are represented,
   with potentially missing work identified separately.
2. Scope Traceability: Work packages align with approved scope.
3. Structure: The hierarchy has three levels, consistent numbering,
   logical decomposition, and no unnecessary task detail.
4. Duplication: Work packages do not overlap or repeat deliverables.
5. Accountability: Level 2 work packages have confirmed or
   explicitly proposed owners and completion criteria.
6. Dependencies: Cross-team interfaces, milestones, testing,
   deployment, and operational transition are addressed.
7. Planning: Relevant work packages can support scheduling,
   cost estimation, and resource allocation.
8. Governance: Unapproved additions and ownership gaps are
   clearly identified for stakeholder decisions.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [UNRESOLVED CRITICAL ITEMS]

Do not invent project scope, work packages, owners, or approvals.
Flag changes requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Business Application — Employee Onboarding Automation

**Scenario:** An IT team is implementing an automated employee onboarding workflow within an existing business application. The current process relies on emails and spreadsheets, resulting in unclear responsibilities and delayed account provisioning.

The Project Manager needs a WBS to organize requirements, development, integrations, testing, and deployment before detailed scheduling.

### Project Context

| Attribute | Details |
|---|---|
| Project | Employee Onboarding Automation |
| Phase | Planning |
| Delivery approach | Hybrid |
| Business objective | Reduce manual onboarding coordination |
| Key deliverables | Digital onboarding workflow, user provisioning integration, notifications, reporting, training, deployment |
| Systems | HR system, identity management platform, existing business application |
| Team | Project Manager, Business Analyst, Developers, QA Lead, IT Operations |
| Major dependency | Identity platform integration |
| Management decision | Validate deliverable coverage, ownership, and dependencies before approving detailed planning |

### Example Input

```text
Project: Employee Onboarding Automation

Business objective:
Reduce manual onboarding coordination and improve
the consistency of employee account provisioning.

Delivery approach: Hybrid

Confirmed scope:
- Implement an onboarding request workflow.
- Integrate approved provisioning requests with the identity platform.
- Send status notifications to relevant stakeholders.
- Provide onboarding status reporting.
- Deliver user documentation and training.
- Deploy the solution into production.

Known workstreams:
Business Analysis
Development
Integration
Quality Assurance
Deployment
Change Management

Systems:
HR system
Identity management platform
Existing business application

Dependencies:
- HR approval of onboarding workflow
- Identity platform API access
- Business-user availability for UAT
- Production environment readiness

Known milestones:
Requirements approval
Integration readiness
SIT completion
UAT acceptance
Production release

Project roles:
Project Manager
Business Analyst
Development Lead
QA Lead
IT Operations
HR Business Owner

Known constraints:
- Limited developer availability
- Identity integration must pass security review
```

### Example Output — Work Breakdown Structure

#### 1. Three-Level WBS

The following is a proposed planning structure based on the supplied scope. Supporting activities are included where necessary to deliver the confirmed capabilities; ownership and approval remain subject to validation.

```text
1.0 Project Management and Governance
    1.1 Project Planning and Control
        1.1.1 Approved delivery plan
        1.1.2 Risk and dependency register
        1.1.3 Project reporting and decision records

2.0 Requirements and Solution Design
    2.1 Business Requirements
        2.1.1 Onboarding process requirements
        2.1.2 Functional acceptance criteria
        2.1.3 Approved workflow requirements

    2.2 Technical Solution Design
        2.2.1 Application design
        2.2.2 Identity integration specification
        2.2.3 Security design review

3.0 Application Development
    3.1 Onboarding Workflow
        3.1.1 Onboarding request functionality
        3.1.2 Approval workflow configuration
        3.1.3 Request status tracking

    3.2 Notifications and Reporting
        3.2.1 Notification functionality
        3.2.2 Status reporting functionality
        3.2.3 Functional validation evidence

4.0 Identity Platform Integration
    4.1 Provisioning Integration
        4.1.1 Interface configuration
        4.1.2 Provisioning request processing
        4.1.3 Integration verification

5.0 Testing and Quality Assurance
    5.1 System Integration Testing
        5.1.1 Integration test cases
        5.1.2 Executed integration tests
        5.1.3 Defect resolution evidence

    5.2 User Acceptance Testing
        5.2.1 UAT scenarios
        5.2.2 Business validation results
        5.2.3 UAT acceptance record

6.0 Business Readiness
    6.1 Documentation and Training
        6.1.1 User documentation
        6.1.2 Training materials
        6.1.3 Completed training sessions

7.0 Deployment and Transition
    7.1 Production Deployment
        7.1.1 Deployment readiness assessment
        7.1.2 Production release
        7.1.3 Post-deployment verification

    7.2 Operational Handover
        7.2.1 Support documentation
        7.2.2 Operational knowledge transfer
        7.2.3 Handover acceptance

8.0 Project Close-Out
    8.1 Project Closure
        8.1.1 Deliverable acceptance summary
        8.1.2 Outstanding action handover
        8.1.3 Project closure report
```

#### 2. Work Package Register

| WBS ID | Work Package | Proposed Owner | Major Dependency | Completion Criterion | Scope Status |
|---|---|---|---|---|---|
| 1.1 | Project Planning and Control | Project Manager | Project governance | Planning and control records accepted | Supporting work proposed |
| 2.1 | Business Requirements | Business Analyst | HR input | Requirements approved | Supporting work proposed |
| 2.2 | Technical Solution Design | Development Lead | Requirements | Design reviewed and accepted | Supporting work proposed |
| 3.1 | Onboarding Workflow | Development Lead | Approved workflow | Agreed workflow criteria met | Confirmed capability; package proposed |
| 3.2 | Notifications and Reporting | Development Lead | Approved requirements | Features meet acceptance criteria | Confirmed capability; package proposed |
| 4.1 | Provisioning Integration | Development Lead | Identity API | Integration tests passed | Confirmed capability; package proposed |
| 5.1 | System Integration Testing | QA Lead | Integrated solution | Required tests completed and evaluated | Supporting work proposed |
| 5.2 | User Acceptance Testing | HR Business Owner | Test readiness | UAT acceptance recorded | Supporting work proposed |
| 6.1 | Documentation and Training | Business Analyst | Approved functionality | Materials and training accepted | Confirmed deliverable; package proposed |
| 7.1 | Production Deployment | IT Operations | Release approval | Deployment verified | Confirmed deliverable; package proposed |
| 7.2 | Operational Handover | IT Operations | Production readiness | Support ownership accepted | Supporting work proposed |
| 8.1 | Project Closure | Project Manager | Delivery acceptance | Closure records approved | Supporting work proposed |

#### 3. WBS Gap Review

| Missing / Unclear Work | Potential Impact | Recommended Location | Proposed Action | Priority |
|---|---|---|---|---|
| HR system data interface | Incomplete onboarding data flow | 2.2 or new integration package | Confirm whether HR data integration is required | High |
| Security approval evidence | Integration or release delay | 2.2 / 7.1 | Define security acceptance requirements | High |
| Failure handling for provisioning | Incomplete operational capability | 4.1 | Clarify retry, exception, and alert requirements | High |
| Rollback preparation | Production recovery risk | 7.1 | Confirm rollback requirements | High |
| Post-launch support arrangements | Unclear incident ownership | 7.2 | Confirm support scope and handover criteria | Medium |

*These gaps are review findings, not approved scope additions.*

#### 4. Cross-Workstream Dependencies

| WBS ID | Dependency | Provider / Proposed Owner | Receiving Work Package | Delivery Impact |
|---|---|---|---|---|
| 2.1 | Approved onboarding requirements | HR Business Owner | 2.2 Solution Design | Design cannot be finalized |
| 4.1 | Identity API access | Identity Platform Team | 4.1 Provisioning Integration | Integration development may be delayed |
| 5.1 | Integrated functionality | Development Lead | 5.1 SIT | Testing cannot complete |
| 5.2 | SIT results and business availability | QA Lead / HR | 5.2 UAT | Business acceptance may be delayed |
| 7.1 | UAT acceptance and release readiness | HR / IT Operations | 7.1 Deployment | Production release at risk |

#### 5. WBS-to-Schedule Mapping

| WBS ID | Work Package | Detailed Scheduling Required? | Key Dependency | Related Milestone |
|---|---|---|---|---|
| 2.1 | Business Requirements | Yes | HR stakeholder availability | Requirements approval |
| 2.2 | Technical Solution Design | Yes | Approved requirements | Design readiness |
| 3.1 | Onboarding Workflow | Yes | Solution design | Development completion |
| 3.2 | Notifications and Reporting | Yes | Agreed feature requirements | Development completion |
| 4.1 | Provisioning Integration | Yes | Identity API access | Integration readiness |
| 5.1 | System Integration Testing | Yes | Integrated build | SIT completion |
| 5.2 | User Acceptance Testing | Yes | SIT completion | UAT acceptance |
| 6.1 | Documentation and Training | Yes | Stable functionality | Business readiness |
| 7.1 | Production Deployment | Yes | Release readiness | Production release |
| 7.2 | Operational Handover | Yes | Support readiness | Handover acceptance |

The mapping identifies work packages that require schedule planning. Detailed activities, durations, and dates must be developed separately.

### Management Decisions

1. **Scope completeness:** Confirm whether HR system integration, exception handling, and rollback requirements must be added to the approved scope.
2. **Ownership:** Assign and validate accountable work package owners and cross-team dependencies.
3. **Schedule readiness:** Prioritize detailed planning for integration, SIT, UAT, and production deployment.
4. **Governance:** Obtain stakeholder approval of the WBS and resolve proposed supporting work before establishing the scope baseline.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The WBS follows the required three-level hierarchy, uses consistent numbering, and covers the principal project deliverables. However, several supporting work packages, ownership assignments, and potential scope gaps require confirmation.

**Required corrections:**
- Validate WBS completeness against approved requirements.
- Confirm whether identified gaps require additional scope.
- Assign work package owners.
- Validate cross-team dependencies and completion criteria.
- Approve the WBS before using it as a planning baseline.

**Approval blockers:** Unconfirmed scope additions, incomplete ownership, and unresolved integration requirements.

**Governance:** This framework supports PMI-aligned scope decomposition, planning, schedule development, resource management, cost estimation, and delivery control.

The WBS is a planning artifact and must be validated by the Project Manager, Business Analyst, Technical Lead, QA Lead, and relevant business stakeholders. Protect confidential project, vendor, personal, and security-sensitive information.
