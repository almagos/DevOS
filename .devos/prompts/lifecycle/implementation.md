# Implementation Workflow Prompt

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Compatible Agents:** ChatGPT, Claude, Codex, Antigravity
>
> **Related Playbook:** `docs/playbooks/implementation.md`
>
> **Related Standards:** `docs/standards/documentation-standard.md`, `docs/standards/repository-standard.md`

---

# Purpose

This prompt executes the DevOS Implementation Playbook.

Its purpose is to implement an approved engineering plan while preserving repository architecture, documentation quality and long-term maintainability.

Implementation follows planning.

It does not replace planning.

---

# Prerequisites

Before executing this prompt ensure that:

- Planning has been completed.
- Scope has been approved.
- Acceptance Criteria have been defined.
- Repository documentation is current.
- Relevant ADRs, standards and patterns have been reviewed.

Implementation should not begin until planning is complete.

---

# Inputs

Provide:

- Approved implementation plan
- Repository
- Relevant documentation
- Related issues
- Existing architecture
- Acceptance Criteria

---

# Prompt

Execute the DevOS Implementation Playbook.

Playbook:

`docs/playbooks/implementation.md`

## Objective

Implement the approved work while preserving repository consistency.

Follow the approved implementation plan.

Reuse existing repository knowledge whenever possible.

Avoid introducing unnecessary complexity.

---

## Implementation Activities

Before making changes:

Review:

- Repository Constitution
- Repository Structure
- Relevant Playbooks
- Relevant Standards
- Relevant Templates
- Relevant ADRs
- Existing Components
- Existing Patterns
- Existing Utilities
- Existing Services

Implement only the approved scope.

---

## Engineering Expectations

The implementation should:

- Follow existing repository patterns.
- Reuse existing components whenever practical.
- Preserve repository architecture.
- Respect established coding standards.
- Maintain accessibility.
- Maintain security.
- Maintain performance.
- Minimize unnecessary dependencies.

---

## Repository Updates

When implementation requires documentation updates:

- Update Canonical Knowledge.
- Update related documentation.
- Maintain repository consistency.
- Avoid duplicate knowledge.

---

## Constraints

Do not change approved architecture.

Do not introduce unrelated refactoring.

Do not expand scope.

Do not duplicate repository knowledge.

Do not modify unrelated files.

---

# Deliverables

Produce:

- Completed implementation
- Updated documentation (if required)
- Tests (if applicable)
- Repository changes consistent with DevOS

---

# Success Criteria

Implementation succeeds when:

- Approved scope has been completed.
- Acceptance Criteria are satisfied.
- Repository standards are followed.
- Existing functionality is preserved.
- Documentation remains synchronized.
- The work is ready for validation.

---

# Related Documentation

## Playbooks

- `docs/playbooks/implementation.md`

## Standards

- `docs/standards/documentation-standard.md`
- `docs/standards/repository-standard.md`

## Templates

- `docs/integrations/linear/issue-template.md`

## Repository Constitution

- `AGENTS.md`
