# Knowledge Synchronization Workflow Prompt

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Compatible Agents:** ChatGPT, Claude, Codex, Antigravity
>
> **Related Playbook:** `docs/playbooks/knowledge-synchronization.md`
>
> **Related Standards:** `docs/standards/documentation-standard.md`, `docs/standards/repository-standard.md`

---

# Purpose

This prompt executes the DevOS Knowledge Synchronization Playbook.

Its purpose is to synchronize Canonical Knowledge with implemented reality after implementation has been validated.

Knowledge Synchronization ensures that repository documentation accurately reflects the current state of the repository.

It maintains the integrity of the repository's Source of Truth.

---

# Prerequisites

Before executing this prompt ensure that:

- Validation has successfully completed.
- Repository changes have been finalized.
- Documentation updates have been identified.
- Repository state accurately reflects the completed work.

Knowledge Synchronization should only occur after successful validation.

---

# Inputs

Provide:

- Validated implementation
- Repository
- Repository changes
- Related issues
- Updated Generated Operational State
- Relevant documentation

---

# Prompt

Execute the DevOS Knowledge Synchronization Playbook.

Playbook:

`docs/playbooks/knowledge-synchronization.md`

## Objective

Synchronize Canonical Knowledge with the validated implementation.

Review repository changes and determine whether documentation requires updates.

Ensure that repository knowledge accurately reflects implemented reality.

---

## Synchronization Activities

Review:

- Repository Constitution
- Repository documentation
- Repository changes
- Generated Operational State
- Related ADRs
- Related Standards
- Related Templates
- Related Playbooks

Identify documentation affected by the implementation.

---

## Documentation Review

Determine whether updates are required to:

- Product documentation
- Engineering documentation
- Operations documentation
- Architecture documentation
- Standards
- Templates
- Playbooks
- Integration documentation
- ADRs
- Glossary

Update only documents affected by the completed implementation.

Avoid unnecessary documentation changes.

---

## Source of Truth Verification

Verify:

- Documentation reflects implemented reality.
- Generated Operational State remains separate from Canonical Knowledge.
- Repository structure remains consistent.
- No duplicate knowledge has been introduced.

---

## Knowledge Synchronization Report

Produce a report describing:

- Repository changes reviewed
- Documentation updated
- Documentation unchanged
- Source of Truth verification
- Outstanding documentation work (if any)

---

## Constraints

Do not introduce new functionality.

Do not redesign repository documentation.

Do not duplicate knowledge.

Update only documentation affected by the completed implementation.

Maintain repository consistency.

---

# Deliverables

Produce:

- Updated Canonical Knowledge (when required)
- Knowledge Synchronization Report
- Documentation update summary

---

# Success Criteria

Knowledge Synchronization succeeds when:

- Canonical Knowledge reflects implemented reality.
- Repository documentation is synchronized.
- Source of Truth remains unambiguous.
- Repository consistency is preserved.
- Documentation drift has been eliminated.

---

# Related Documentation

## Playbooks

- `docs/playbooks/knowledge-synchronization.md`

## Standards

- `docs/standards/documentation-standard.md`
- `docs/standards/repository-standard.md`

## Repository Constitution

- `AGENTS.md`

## Generated Operational State

- `.devos/`
