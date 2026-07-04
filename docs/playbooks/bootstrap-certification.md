# Bootstrap Certification Playbook

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Repository Certification
>
> This playbook defines the process for certifying that a repository is capable of onboarding autonomous AI agents and human contributors using only its documented knowledge.

---

# Purpose

Bootstrap Certification validates that a repository is:

- Self-describing
- Internally consistent
- AI-onboardable
- Human-onboardable
- Architecturally complete

The objective is to determine whether the repository contains sufficient knowledge for a new contributor to understand how work is performed without relying on undocumented context.

Bootstrap Certification evaluates repository architecture rather than implementation.

---

# When to Run

Bootstrap Certification should be performed:

- Before the first public release of a repository.
- After major architectural changes.
- Before publishing a repository as a GitHub Template.
- Periodically to detect documentation drift.
- After significant repository restructuring.

---

# Inputs

Bootstrap Certification uses:

- AGENTS.md
- Repository Constitution
- Documentation Architecture
- Repository Structure
- Glossary
- Playbooks
- Standards
- Templates
- Integration Documentation
- Domain Documentation
- Generated Operational State

No external knowledge should be required.

---

# Workflow

```
Start

↓

Read AGENTS.md

↓

Traverse Documentation

↓

Validate Navigation

↓

Validate Architecture

↓

Validate Terminology

↓

Validate Workflows

↓

Validate Integrations

↓

Validate Generated Operational State

↓

Assess AI Onboarding

↓

Produce Certification Report

↓

End
```

---

# Certification Process

The certification process consists of the following stages.

## Stage 1 — Repository Bootstrap

Begin with:

`AGENTS.md`

Follow every referenced document recursively until no additional repository documentation remains.

Do not use repository history or external knowledge.

---

## Stage 2 — Navigation Validation

Verify:

- Every referenced document exists.
- Every document is reachable.
- Every README supports repository navigation.
- No dead ends exist.
- No broken internal references exist.

---

## Stage 3 — Documentation Architecture Validation

Verify:

- Repository Constitution
- Glossary
- Contracts
- Playbooks
- Standards
- Templates
- Integrations
- Domain Knowledge
- Generated Operational State

Ensure responsibilities remain clearly separated.

---

## Stage 4 — Workflow Validation

Reconstruct the repository lifecycle.

Verify:

Planning

↓

Implementation

↓

Validation

↓

Knowledge Synchronization

↓

Release

Confirm that each stage has:

- clear purpose
- inputs
- outputs
- entry criteria
- exit criteria

---

## Stage 5 — Terminology Validation

Use the Glossary as the canonical vocabulary.

Verify:

- terminology consistency
- absence of conflicting concepts
- absence of undefined critical concepts
- absence of duplicate terminology

---

## Stage 6 — Integration Validation

Review every integration.

Verify:

- responsibility boundaries
- Source of Truth ownership
- alignment with DevOS architecture
- repository consistency

---

## Stage 7 — Generated Operational State Validation

Review the `.devos` directory.

Verify:

- separation from Canonical Knowledge
- reproducibility
- automation readiness
- AI usability

---

## Stage 8 — AI Onboarding Validation

Determine whether an autonomous coding agent can confidently answer:

- What is this repository?
- How does work begin?
- How is planning performed?
- How is implementation performed?
- How is validation performed?
- How does documentation evolve?
- Where does knowledge belong?
- Where does operational state belong?
- Which systems are Sources of Truth?

Document every required assumption.

---

## Stage 9 — Certification

Produce the final certification.

Possible outcomes:

- ✅ DevOS Certified
- ⚠️ DevOS Certified with Recommendations
- ❌ DevOS Not Yet Ready

---

# Deliverables

Bootstrap Certification produces:

- Bootstrap Trace
- Navigation Audit
- Documentation Architecture Audit
- Workflow Audit
- Terminology Audit
- Integration Audit
- Generated Operational State Audit
- AI Onboarding Audit
- Recommendations
- Final Certification

---

# Success Criteria

Bootstrap Certification succeeds when:

- Every repository document is reachable.
- Repository navigation is deterministic.
- Repository terminology is consistent.
- Workflows are reconstructible.
- Sources of Truth are unambiguous.
- AI onboarding requires no undocumented knowledge.
- Documentation architecture is internally consistent.

---

# Failure Criteria

Certification fails when any of the following occur:

- Broken repository navigation.
- Missing repository documentation.
- Conflicting Sources of Truth.
- Undefined critical terminology.
- Ambiguous workflows.
- Architectural inconsistencies.
- Missing repository responsibilities.

---

# Related Documents

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

---

## Repository Vocabulary

- `docs/glossary.md`

---

## Related Playbooks

- `planning.md`
- `implementation.md`
- `validation.md`
- `knowledge-synchronization.md`
- `release.md`

---

## Related Standards

- `docs/standards/documentation-standard.md`
- `docs/standards/repository-standard.md`

---

## Related Templates

- `docs/templates/playbook-template.md`


Bootstrap Certification evaluates the repository at a point in time.

Any material changes to repository architecture, documentation, playbooks, standards, templates or integrations invalidate previous certification results and require re-certification.
