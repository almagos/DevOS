# Linear Issue Template

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Linear Integration
>
> This template defines the canonical structure for Parent Issues and Child Issues authored within Linear.
>
> All Linear planning artifacts should follow this structure.

---

# Purpose

This template defines the canonical structure for Parent Issues and Child Issues authored within Linear.

It ensures planning artifacts are:

- Consistent
- Complete
- Unambiguous
- AI-friendly

Each issue should describe exactly one planning artifact.

Implementation details belong in source code and repository documentation rather than planning artifacts.

---

# Repository References

This template is governed by the following repository documentation.

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

## Repository Vocabulary

- `docs/glossary.md`

## Related Playbooks

- `docs/playbooks/planning.md`

## Related Standards

- `docs/integrations/linear/authoring-standard.md`

---

# Relationship to DevOS

This template supports the Planning lifecycle stage.

It defines the structure of planning artifacts stored in Linear.

Repository documentation should not duplicate planning artifacts.

Canonical Knowledge is created through the Knowledge Synchronization workflow after implementation and validation have completed.

---

# Authoring Rules

Every Linear Issue MUST:

- Describe exactly one Parent Issue or one Child Issue.
- Define a single planning objective.
- Be independently understandable.
- Contain sufficient context for autonomous coding agents.
- Reference existing repository knowledge rather than duplicating it.
- Define measurable acceptance criteria.
- Use repository terminology defined in the Glossary.

The issue MUST NOT:

- Introduce unrelated work.
- Duplicate ADRs.
- Duplicate architecture documentation.
- Duplicate implementation details already documented elsewhere.
- Describe implementation history.

---

# Writing Guidelines

Every section should be:

- Concise
- Deterministic
- Implementation-oriented
- Independently understandable

Prefer bullet points over long paragraphs.

Avoid repetition.

Reference repository documentation instead of duplicating it.

Every statement should help a coding agent understand the planning intent.

Avoid marketing language, opinions and unnecessary explanation.

---

# Objective

Describe the single outcome this issue is intended to achieve.

---

# Background

Provide the context required to understand why this work exists.

Reference existing repository documentation whenever possible.

---

# Problem Statement

Describe the problem this issue solves.

Focus on the problem rather than the implementation.

---

# Scope

List everything included in this issue.

---

# Out of Scope

List everything intentionally excluded.

---

# User Flows

Describe expected behaviour.

When applicable include:

- Entry Point
- Happy Path
- Empty State
- Loading State
- Error State
- Permission Scenarios
- Edge Cases
- Desktop
- Tablet
- Mobile

If the feature has no user interface, describe the operational or API flow instead.

---

# Functional Requirements

Describe the required behaviour of the system.

Prefer concise bullet points.

---

# Implementation Guidance

Provide implementation guidance that is specific to this feature and repository.

Examples include:

- Existing components to reuse
- Existing patterns to follow
- Existing services or utilities to extend
- Files or modules likely to change
- Performance expectations
- Accessibility expectations
- Security expectations
- Documentation expected after implementation
- Architectural decisions to follow
- Behaviours to avoid

Avoid generic guidance that applies to every issue.

The objective of this section is to reduce ambiguity while preserving implementation flexibility.

---

# Constraints

The implementation MUST NOT:

- Break existing functionality.
- Introduce unrelated refactoring.
- Modify approved architecture.
- Duplicate repository knowledge.
- Introduce unnecessary dependencies.

---

# Dependencies

List relevant dependencies.

Examples:

- Parent Issue
- Child Issues
- ADRs
- Standards
- Architecture Documents
- External Services
- External APIs

---

# Repository Impact

Describe expected repository changes.

Examples:

- New Pages
- New Components
- New Routes
- New APIs
- Database Migrations
- Storage Changes
- Tests
- Documentation
- Configuration

---

# Deliverables

List the expected outputs.

Examples:

- UI completed
- API completed
- Database migration
- Tests added
- Repository documentation synchronized

---

# Acceptance Criteria

Define measurable acceptance criteria.

Each criterion should be independently verifiable.

---

# Verification

Describe how implementation should be verified.

Examples:

- Manual Testing
- Automated Tests
- Mobile Testing
- Cross Browser Testing
- Performance Validation
- Security Validation

---

# Risks

Document known risks, assumptions and trade-offs.

---

# Definition of Done

The issue is complete when:

- Acceptance Criteria have been satisfied.
- Implementation has been completed.
- Required validation has passed.
- No known regressions remain.
- The issue is ready for Knowledge Synchronization.

---

# Context References

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

---

## Repository Vocabulary

- `docs/glossary.md`

---

## Related Playbooks

Examples:

- Planning
- Implementation
- Validation

---

## Related Standards

Examples:

- Documentation Standard
- Repository Standard
- Writing Standard
- Naming Standard

---

## Related Architecture

List architecture documents, ADRs, patterns or specifications that define implementation expectations.

Examples:

- Architecture documents
- ADRs
- Patterns
- Repository specifications

Only include references that are directly relevant to implementing this issue.

---

## Related Issues

List related Parent Issues or Child Issues.

Examples:

- Parent Issue
- Dependency Issues
- Supporting Issues

---

## Design References

List design artifacts when applicable.

Examples:

- Figma
- Wireframes
- Prototypes
- UX Specifications

Only include references directly relevant to this issue.
