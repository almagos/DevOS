# Validation Workflow Prompt

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Compatible Agents:** ChatGPT, Claude, Codex, Antigravity
>
> **Related Playbook:** `docs/playbooks/validation.md`
>
> **Related Standards:** `docs/standards/documentation-standard.md`, `docs/standards/repository-standard.md`

---

# Purpose

This prompt executes the DevOS Validation Playbook.

Its purpose is to verify that completed implementation satisfies the approved requirements, acceptance criteria and repository standards before work proceeds to Knowledge Synchronization and Release.

Validation evaluates implementation.

It does not implement new functionality.

---

# Prerequisites

Before executing this prompt ensure that:

- Implementation has been completed.
- Acceptance Criteria have been defined.
- Documentation has been updated where required.
- Relevant tests have been completed or are available for review.

Validation should only begin after implementation is complete.

---

# Inputs

Provide:

- Completed implementation
- Approved implementation plan
- Acceptance Criteria
- Repository
- Relevant documentation
- Related issues

---

# Prompt

Execute the DevOS Validation Playbook.

Playbook:

`docs/playbooks/validation.md`

## Objective

Verify that the completed implementation satisfies the approved plan and is ready to proceed to Knowledge Synchronization.

Validation should confirm implementation quality without expanding scope.

---

## Validation Activities

Review:

- Approved implementation plan
- Acceptance Criteria
- Repository Constitution
- Repository Standards
- Documentation updates
- Repository changes
- Tests
- Related ADRs
- Related Patterns

---

## Validation Requirements

Verify:

- Acceptance Criteria are satisfied.
- Scope matches the approved plan.
- Repository standards have been followed.
- Existing functionality has not regressed.
- Documentation is synchronized.
- Repository structure remains consistent.
- No undocumented architectural changes have been introduced.

---

## Quality Checks

Evaluate:

- Functional correctness
- Repository consistency
- Documentation quality
- Naming consistency
- Accessibility
- Security
- Performance
- Error handling
- Test coverage (when applicable)

---

## Validation Result

Determine one of the following outcomes:

- ✅ Passed
- ⚠️ Passed with Recommendations
- ❌ Failed

Provide justification for the outcome.

---

## Constraints

Do not implement new functionality.

Do not expand scope.

Do not introduce architectural changes.

Only identify issues and recommendations.

---

# Deliverables

Produce a Validation Report containing:

- Executive Summary
- Validation Findings
- Acceptance Criteria Review
- Repository Compliance
- Quality Assessment
- Recommendations
- Validation Result

---

# Success Criteria

Validation succeeds when:

- Acceptance Criteria have been objectively evaluated.
- Repository standards have been verified.
- Documentation is synchronized.
- Repository consistency has been preserved.
- A clear validation outcome has been produced.

---

# Related Documentation

## Playbooks

- `docs/playbooks/validation.md`

## Standards

- `docs/standards/documentation-standard.md`
- `docs/standards/repository-standard.md`

## Templates

- `docs/templates/specification-template.md`

## Repository Constitution

- `AGENTS.md`
