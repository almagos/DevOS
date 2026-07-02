# Linear Issue Template

Version: 1.0

Status: Active

Owner: DevOS

---

# Purpose

This document defines the canonical template for the Markdown stored in the `description` field of every Linear Issue.

Every Linear Issue MUST describe exactly one independently implementable feature.

The completed template is serialized unchanged into the Linear Issue `description` field.

---

# Repository References

Creation and serialization of this template are governed by:

`standards/linear-authoring-standard.md`

---

# Authoring Rules

Every Linear Issue MUST:

- describe exactly one feature
- be independently implementable
- contain sufficient context for autonomous coding agents
- reference existing repository knowledge instead of duplicating it
- avoid ambiguity
- define measurable outcomes

The issue MUST NOT:

- introduce unrelated work
- duplicate ADRs
- duplicate architecture documentation
- duplicate implementation details already documented elsewhere

---

# Writing Guidelines

Every section should be:

- concise
- deterministic
- implementation-oriented
- independently understandable

Prefer bullet points over long paragraphs.

Avoid repetition.

Reference repository documents instead of duplicating them.

Every statement should help a coding agent implement the feature.

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

Avoid discussing implementation.

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

# Engineering Requirements

Describe engineering expectations.

Examples:

- Authentication
- Authorization
- Database
- Storage
- APIs
- Rendering
- Performance
- Accessibility
- Security
- Observability
- Logging
- Monitoring
- Caching

Do not prescribe implementation unless already approved.

---

# Constraints

The implementation MUST NOT:

- break existing functionality
- introduce unrelated refactoring
- modify approved architecture
- duplicate repository knowledge
- introduce unnecessary dependencies

---

# Dependencies

List:

- Related Linear Issues
- ADRs
- Standards
- Patterns
- External Dependencies

---

# Repository Changes

Describe expected repository modifications.

Examples:

- New Pages
- New Components
- New Routes
- New APIs
- Database Migrations
- Storage Changes
- Tests
- Documentation

---

# Deliverables

List the expected outputs.

Examples:

- UI completed
- API completed
- Database migration
- Tests added
- Documentation updated

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

- Acceptance Criteria satisfied
- Implementation completed
- Tests passing
- Documentation updated
- No known regressions
- Ready for review

---

# Engineering Instructions

Provide implementation guidance that is specific to this feature and repository.

Include repository-specific expectations where applicable, such as:

- Existing components to reuse
- Existing patterns to follow
- Existing services or utilities to extend
- Files or modules likely to change
- Performance expectations
- Accessibility expectations
- Security expectations
- Coding standards to follow
- Documentation updates required
- Behaviors or architectural decisions to avoid

Avoid generic guidance that applies to every issue. The objective of this section is to help autonomous coding agents implement this feature consistently with the repository architecture while minimizing ambiguity and unnecessary implementation decisions.

---

# Context References

## Repository Standards

List the repository standards that govern implementation.

Examples

- standards/linear-authoring-standard.md
- standards/templates/linear-issue-template.md

---

## Related Issues

List related Linear Issues that provide implementation context.

Examples

- Parent Issue
- Prototype Issue
- Supporting Architecture
- Dependency Issues

---

## Architecture References

List architecture documents, ADRs, patterns or requirements that define implementation expectations.

Examples

- docs/architecture/*
- docs/patterns/*
- docs/decisions/*
- docs/requirements/*

---

## Design References

List UI prototypes, mockups or design artifacts that define the expected user experience.

Examples

- ALM-44 — Artifact Viewer Prototype

Only include references that are directly relevant to implementing this issue.
