# Release Workflow Prompt

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Compatible Agents:** ChatGPT, Claude, Codex, Antigravity
>
> **Related Playbook:** `docs/playbooks/release.md`
>
> **Related Standards:** `docs/standards/repository-standard.md`

---

# Purpose

This prompt executes the DevOS Release Playbook.

Its purpose is to determine whether validated and synchronized work is ready for release and to execute the repository release process.

Release represents the completion of a development lifecycle.

It should only occur after successful Planning, Implementation, Validation and Knowledge Synchronization.

---

# Prerequisites

Before executing this prompt ensure that:

- Planning has completed.
- Implementation has completed.
- Validation has passed.
- Knowledge Synchronization has completed.
- Repository documentation reflects implemented reality.

---

# Inputs

Provide:

- Repository
- Completed implementation
- Validation results
- Knowledge Synchronization Report
- Release target
- Related issues

---

# Prompt

Execute the DevOS Release Playbook.

Playbook:

`docs/playbooks/release.md`

## Objective

Determine whether the repository changes are ready for release.

Verify repository quality before publishing.

Confirm that all release requirements have been satisfied.

---

## Release Activities

Review:

- Repository Constitution
- Validation results
- Knowledge Synchronization Report
- Repository documentation
- Repository structure
- Related issues
- Release notes (if applicable)

---

## Release Verification

Verify:

- Acceptance Criteria have been satisfied.
- Validation has passed.
- Documentation is synchronized.
- Repository standards have been followed.
- Repository structure remains consistent.
- Source of Truth remains unambiguous.
- Release artifacts are complete.

---

## Release Readiness

Determine one of the following outcomes:

- ✅ Ready for Release
- ⚠️ Ready with Recommendations
- ❌ Not Ready for Release

Provide justification.

---

## Release Deliverables

When applicable produce:

- Release Summary
- Release Notes
- Version Recommendation
- Repository Tag Recommendation
- Outstanding Follow-up Work

---

## Constraints

Do not introduce new functionality.

Do not expand scope.

Do not redesign architecture.

Evaluate only release readiness.

---

# Deliverables

Produce a Release Readiness Report containing:

- Executive Summary
- Release Verification
- Repository Readiness
- Outstanding Items
- Recommendations
- Release Decision

---

# Success Criteria

Release succeeds when:

- Repository quality has been verified.
- Documentation reflects implemented reality.
- Repository standards have been followed.
- Repository is ready for publication or deployment.
- A clear release decision has been produced.

---

# Related Documentation

## Playbooks

- `docs/playbooks/release.md`

## Standards

- `docs/standards/repository-standard.md`

## Repository Constitution

- `AGENTS.md`

## Generated Operational State

- `.devos/`
