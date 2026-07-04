# Planning Workflow Prompt

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Compatible Agents:** ChatGPT, Claude, Codex, Antigravity
>
> **Related Playbook:** `docs/playbooks/planning.md`
>
> **Related Standards:** `docs/standards/documentation-standard.md`, `docs/standards/repository-standard.md`

---

# Purpose

This prompt executes the DevOS Planning Playbook.

Its purpose is to transform an approved idea, requirement or request into an implementation-ready engineering plan.

Planning establishes a shared understanding before implementation begins.

The planning process does not produce implementation.

---

# Prerequisites

Before executing this prompt ensure that:

- The problem or requirement has been clearly described.
- Relevant repository documentation is available.
- Existing architecture has been reviewed.
- Related ADRs, standards and patterns have been identified.

---

# Inputs

Provide:

- Repository
- Requirement, feature request or problem statement
- Relevant repository documentation
- Existing architecture
- Related issues (if applicable)

---

# Prompt

Execute the DevOS Planning Playbook.

Playbook:

`docs/playbooks/planning.md`

## Objective

Produce a complete implementation plan for the requested work.

The plan should eliminate ambiguity before implementation begins.

Reuse existing repository knowledge whenever possible.

---

## Planning Activities

Review:

- Repository Constitution
- Repository Architecture
- Repository Structure
- Relevant Playbooks
- Relevant Standards
- Relevant Templates
- Related ADRs
- Existing Patterns
- Existing Components
- Existing APIs
- Existing Integrations

Avoid duplicating repository knowledge.

---

## Planning Deliverables

Produce:

- Objective
- Background
- Problem Statement
- Scope
- Out of Scope
- User Flows (if applicable)
- Functional Requirements
- Engineering Requirements
- Constraints
- Dependencies
- Repository Changes
- Deliverables
- Acceptance Criteria
- Verification Strategy
- Risks
- Engineering Instructions
- Context References

The resulting plan should be implementation-ready.

---

## Constraints

Do not implement code.

Do not make architectural decisions that have not been approved.

Reference existing repository documentation instead of duplicating it.

---

# Deliverables

Produce a complete implementation plan suitable for creating:

- Linear Issues
- GitHub Issues
- Feature Specifications

---

# Success Criteria

The planning workflow succeeds when:

- Repository context has been reviewed.
- Scope is clearly defined.
- Acceptance Criteria are measurable.
- Dependencies are identified.
- Implementation ambiguity has been minimized.
- The work is ready for implementation.

---

# Related Documentation

## Playbooks

- `docs/playbooks/planning.md`

## Standards

- `docs/standards/documentation-standard.md`
- `docs/standards/repository-standard.md`

## Templates

- `docs/integrations/linear/issue-template.md`
- `docs/templates/specification-template.md`

## Repository Constitution

- `AGENTS.md`
