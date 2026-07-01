# DAS-04 — WHO

| Metadata | Value |
| --- | --- |
| **Title** | DAS-04 — WHO |
| **Document ID** | DAS-04 |
| **Version** | 1.0.0 |
| **Status** | Approved |
| **Parent** | AF-001 — DevOS Foundation Architecture |
| **Last Updated** | 2026-07-01 |

---

## Purpose

The WHO dimension defines the roles that participate in DevOS, their responsibilities, interactions and accountability throughout the software development lifecycle.

---

## Principles

- Roles represent responsibilities rather than people or tools.
- One person may perform multiple roles.
- One role may be performed by different humans or AI systems over time.
- DevOS defines responsibilities, not job titles.

---

## Core Roles

- Product Manager: defines requirements, produces and approves specifications, prioritizes work.
- Work Manager: creates issues, publishes engineering contracts, tracks execution.
- Engineering Executor: implements approved engineering contracts, updates repository artifacts, opens pull requests.
- Reviewer: validates correctness, scope, documentation and standards.
- Integrator: merges approved pull requests and maintains repository integrity.

---

## Supporting Roles

- Stakeholder: provides business and domain input.
- User: consumes the product and generates future work through feedback.

---

## Responsibility Rules

- Responsibilities have one primary owner.
- Execution may be delegated.
- Accountability may not be delegated.

---

## Core Rules

- Planning is separated from implementation.
- Implementation is separated from review.
- Review is separated from integration.
- Roles are tool-independent.
- AI and humans may perform the same role.

---

## Success Criteria

Every responsibility has a primary owner, roles remain tool-independent, responsibilities are clearly separated, and accountability remains explicit.
