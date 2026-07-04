# AGENTS.md

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Entire Repository
>
> This document is the bootstrap guide for every AI agent working in this repository.
>
> Read this document before making any changes.

---

# 1. Mission

Your objective is to evolve this repository while preserving its architectural integrity.

This repository follows **DevOS**, a knowledge-first development operating system.

Repository knowledge is considered a first-class artifact.

Every change should improve one or more of the following:

- Product
- Engineering
- Operations
- Repository Knowledge

---

# 2. Core Principles

Always preserve these principles.

- Repository knowledge is a first-class artifact.
- Repository documentation reflects implemented reality.
- Every document has exactly one canonical home.
- Reuse existing knowledge before creating new knowledge.
- Prefer consistency over novelty.
- Prefer simplicity over cleverness.
- Preserve long-term maintainability.

---

# 3. Repository Navigation

Before starting any task, read repository knowledge in the following order.

## Level 0

```
AGENTS.md
```

---

## Level 1 — Repository Constitution

Read completely.

```
docs/engineering/repository/documentation-architecture.md

docs/engineering/repository/repository-structure.md
```

---

## Level 2 — Workflow

Read the playbook relevant to your task.

```
docs/playbooks/
```

---

## Level 3 — Standards

Read only applicable standards.

```
docs/standards/
```

---

## Level 4 — Templates

Use the correct template before creating recurring documentation.

```
docs/templates/
```

---

## Level 5 — Domain Knowledge

Read only documentation related to your task.

```
docs/product/

docs/engineering/

docs/operations/
```

---

## Level 6 — Assigned Task

Retrieve the assigned work item from the configured Work Management System.

Only after understanding both the repository knowledge and the assigned work item should implementation begin.

---

# 4. Standard Workflow

Every task follows the same lifecycle.

```
Understand

↓

Plan

↓

Implement

↓

Validate

↓

Knowledge Synchronization

↓

Complete
```

Refer to the corresponding playbook for detailed workflow instructions.

---

# 5. Repository Systems

This repository integrates with external systems that act as Sources of Truth for specific responsibilities.

Always retrieve information from the appropriate system rather than inferring or recreating it.

| Responsibility | System | Purpose |
|---------------|--------|---------|
| Work Management | Linear | Requirements, planning, issue tracking and implementation contracts |
| Source Control | GitHub | Source code, pull requests, releases and version history |
| Repository Knowledge | Repository Documentation | Canonical product, engineering and operational knowledge |
| Generated Operational State | `.devos/` | Generated reports, prompts, metadata and operational artifacts |

Repository documentation remains the canonical Source of Truth for knowledge.

External systems provide operational context but do not replace repository knowledge.

---

# 6. Working Rules

## Repository

- Follow the documented repository architecture.
- Do not invent repository structure.
- Do not create undocumented top-level directories.

---

## Knowledge

- Preserve one source of truth.
- Prefer references over duplication.
- Keep documentation synchronized with implementation.

---

## Documentation

- Document implemented reality.
- Do not document speculative work.
- Do not store planning information as repository knowledge.

---

## Architecture

- Reuse existing patterns.
- Follow documented architecture decisions.
- Preserve repository consistency.

---

## Generated State

`.devos/` contains generated operational state.

- Never treat it as repository knowledge.
- Never manually edit generated artifacts unless explicitly instructed.

---

# 7. When Unsure

When repository knowledge is insufficient, consult the appropriate Repository System before making assumptions.

1. Search existing documentation.
2. Reuse existing patterns.
3. Follow repository conventions.
4. Make the smallest reasonable change.
5. Retrieve missing operational context from the configured Repository System.
6. Do not invent new architecture.
7. Escalate uncertainty rather than guessing.

---

# 8. Definition of Done

A task is complete only when all applicable conditions are satisfied.

- Requirements implemented.
- Validation completed.
- Documentation synchronized.
- Standards satisfied.
- No architectural violations.
- Ready for review.

---

# 9. Forbidden Actions

Never:

- Create duplicate knowledge.
- Create undocumented repository structure.
- Treat planning information as repository documentation.
- Treat `.devos/` as a source of truth.
- Manually edit generated operational artifacts.
- Bypass documented playbooks.
- Ignore repository standards.
- Introduce architectural changes without updating the corresponding documentation.

---

# 10. Decision Priority

When multiple sources appear to conflict, use the following precedence.

1. AGENTS.md
2. Documentation Architecture
3. Repository Structure
4. Relevant Playbook
5. Relevant Standards
6. Relevant Templates
7. Repository Systems
8. Domain Documentation
9. Assigned Work Item

Repository Systems provide operational context.

Repository Documentation remains the canonical Source of Truth.

---

# 11. Continuous Improvement

If implementation exposes weaknesses in DevOS:

1. Improve the repository architecture.
2. Update affected documentation.
3. Update playbooks if workflows change.
4. Update standards if rules change.
5. Update templates if document structures change.

Architectural evolution should be deliberate and infrequent.


This document intentionally contains minimal repository knowledge.

Its purpose is to bootstrap navigation to the canonical documentation rather than duplicate it.
