# GitHub Integration

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** GitHub Integration
>
> This directory contains the GitHub integration documentation for DevOS.
>
> It defines how DevOS workflows map to GitHub and establishes the conventions used by both human contributors and AI agents.

---

# Purpose

GitHub is the Source of Truth for implementation.

This integration defines how DevOS performs implementation activities using GitHub.

Planning remains the responsibility of Linear.

Repository knowledge remains the responsibility of repository documentation.

---

# Responsibilities

GitHub is responsible for:

- Source Code
- Branches
- Commits
- Pull Requests
- Code Review
- Merge History

GitHub is not responsible for:

- Planning
- Product Documentation
- Repository Standards
- Repository Playbooks
- Canonical Knowledge

---

# DevOS ↔ GitHub Mapping

| DevOS | GitHub |
|--------|---------|
| Parent Issue | Linked through Pull Requests |
| Child Issue | Branch + Pull Request |
| Implementation | Commit History |
| Validation | Pull Request Review |
| Knowledge Synchronization | Post-merge workflow |
| Release | Git Tags / Releases |

---

# Repository Standards

GitHub activity is governed by the following documents.

## Standards

- `commit-standard.md`
- `pull-request-standard.md`

## Templates

- `pull-request-template.md`

---

# Relationship to DevOS

GitHub supports the following lifecycle stages.

```
Planning (Linear)

↓

Implementation (GitHub)

↓

Validation (GitHub)

↓

Knowledge Synchronization (Repository)

↓

Release
```

GitHub stores implementation history.

Repository documentation stores Canonical Knowledge.

Linear stores planning.

---

# Source of Truth

| Information | Source of Truth |
|-------------|-----------------|
| Planning | Linear |
| Source Code | GitHub |
| Canonical Knowledge | Repository Documentation |
| Operational State | `.devos/` |

---

# Guiding Principles

- One Pull Request should implement one Child Issue.
- Pull Requests should remain small and independently reviewable.
- Commits should be atomic.
- Repository documentation should not be updated manually during implementation unless required by the active playbook.
- Knowledge Synchronization occurs after implementation and validation.

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

- `docs/playbooks/implementation.md`
- `docs/playbooks/validation.md`
- `docs/playbooks/knowledge-synchronization.md`
- `docs/playbooks/release.md`

---

## Related Standards

- `commit-standard.md`
- `pull-request-standard.md`

---

## Related Templates

- `pull-request-template.md`
