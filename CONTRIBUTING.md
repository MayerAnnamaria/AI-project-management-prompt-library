
# Contribution and Development Guidelines

This document defines the development, version control,
quality assurance, and governance standards for the
AI Project Management Prompt & Decision Framework Library.

## 1. Version Control

Git is the primary source of change history.
Significant changes and release milestones are documented
in [CHANGELOG.md](CHANGELOG.md).

The library follows a versioning convention inspired by
[Semantic Versioning](https://semver.org/).

### Versioning Standard

| Version | Change Type | Example |
|---|---|---|
| MAJOR | Breaking changes to established interfaces or structures | 1.0.0 → 2.0.0 |
| MINOR | New functionality or backward-compatible improvements | 0.1.0 → 0.2.0 |
| PATCH | Corrections and minor non-breaking improvements | 0.0.1 → 0.0.2 |

The initial development baseline is `0.0.1`.
Versions below `1.0.0` represent an evolving library
and do not imply production readiness.

Individual prompt versions are updated when their
content or functionality changes. Repository release
versions represent the overall library baseline.

## 2. Commit Message Standard

Commit messages must be concise, descriptive,
and specific to the affected asset or change.

### Initial Baseline

`Initial Draft (v0.0.1): [Document Name]`

### Subsequent Changes

| Change Type | Example Commit Message |
|---|---|
| Addition | Add release readiness assessment prompt |
| Improvement | Improve risk register scoring criteria |
| Correction | Fix inconsistent risk classification |
| Documentation | Update prompt development guidelines |
| Validation | Add risk register validation scenarios |
| Security | Strengthen confidentiality safeguards |
| Release | Release v0.1.0 |

Each commit should represent one logical change.

## 3. Branching and Change Management

During initial development, minor changes may be
committed directly to the `main` branch.

Material changes and external contributions should
use dedicated branches and pull requests.

| Branch | Purpose |
|---|---|
| main | Primary repository baseline |
| feature/[name] | New functionality or prompts |
| fix/[name] | Defect corrections |
| docs/[name] | Documentation improvements |
| test/[name] | Validation and regression tests |

Changes must be reviewed against the applicable
quality criteria before merging.

## 4. Prompt Configuration Standard

Each operational prompt must include:

- Unique Prompt ID
- Category
- Version
- Lifecycle status
- Validation status

Supporting methodology documents use a Document ID
where appropriate.

Existing identifiers must remain stable throughout
the asset lifecycle and must not be reused.

### Lifecycle Status

| Status | Definition |
|---|---|
| Initial Draft | Initial development baseline |
| In Review | Under structured review |
| Approved | Meets defined approval criteria |
| Deprecated | Scheduled for retirement |
| Archived | Retained for historical reference |

### Validation Status

| Status | Definition |
|---|---|
| Pending | Formal validation not completed |
| In Progress | Validation underway |
| Passed | Defined acceptance criteria satisfied |
| Failed | One or more acceptance criteria not satisfied |

Material prompt changes require reassessment
of the validation status.

## 5. Quality Assurance

Before committing or merging changes:

- [ ] Verify prompt identification and version metadata.
- [ ] Confirm consistent formatting and document structure.
- [ ] Check factual accuracy and internal consistency.
- [ ] Verify references and repository links.
- [ ] Review confidentiality and human accountability controls.
- [ ] Evaluate affected prompts against relevant test scenarios.
- [ ] Update validation status where applicable.
- [ ] Update the changelog for significant changes.

Validation results must be based on documented evidence.

## 6. AI Governance

All AI-generated outputs require appropriate human review.

Contributors must:

- Protect confidential and restricted information.
- Use authorized data and AI environments.
- Distinguish verified facts from assumptions.
- Identify unsupported AI-generated claims.
- Preserve human decision and approval authority.

AI-generated recommendations must not replace
professional judgment or formal approval.

## 7. Release Management

Before creating a repository release:

1. Confirm the intended release scope.
2. Review outstanding defects and limitations.
3. Verify affected prompt versions.
4. Review applicable quality assurance results.
5. Update the repository version.
6. Finalize the changelog.
7. Create the corresponding Git tag and GitHub release.

Known limitations must be disclosed in release notes.

## 8. Continuous Improvement

The library follows an iterative development approach.

Future improvements may include automated metadata
validation, structured prompt testing, regression
testing, and cross-model compatibility assessments.

---

**Development principle:** Maintain traceability,
reusability, quality, and human accountability
throughout the prompt lifecycle.
