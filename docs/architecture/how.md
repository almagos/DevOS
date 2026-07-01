# DAS-03 — HOW

| Metadata | Value |
| --- | --- |
| **Title** | DAS-03 — HOW |
| **Document ID** | DAS-03 |
| **Version** | 1.0.0 |
| **Status** | Approved |
| **Parent** | AF-001 — DevOS Foundation Architecture |
| **Last Updated** | 2026-07-01 |

---

## Purpose

The HOW dimension defines how work flows through DevOS. It specifies the operating model that transforms an idea into a completed implementation while keeping planning, execution, review and documentation synchronized.

---

## Workflow

Idea → Discussion → Specification → Approval → Engineering Contract → Implementation → Pull Request → Review → Merge → Completion

---

## Workflow Stages

1. Idea – identify new work.
2. Discussion – refine intent; no permanent artifacts.
3. Specification – define what will be implemented.
4. Approval – freeze behavior for the iteration.
5. Engineering Contract – publish Objective, Approved Specification, Repository Changes, Deliverables, Definition of Done and Engineering Instructions.
6. Implementation – implement only the approved specification.
7. Pull Request – submit one primary PR.
8. Review – validate correctness, scope, documentation and standards.
9. Merge – repository becomes the canonical source of truth.
10. Completion – mark the issue Done.

---

## Responsibilities

- Product Manager: define and approve specifications.
- Work Manager: publish engineering contracts and track work.
- Engineering Executor: implement approved work.
- Reviewer: validate implementation.
- Integrator: merge approved work.

---

## Core Rules

- One Issue → One Primary Pull Request.
- GitHub repository is the permanent source of truth after merge.
- Implementation begins only after an approved engineering contract exists.
- Discussions are temporary; approved knowledge is version controlled.
- Documentation evolves together with implementation.
- Every significant change is traceable: Issue → Branch → Commit → Pull Request → Merge → Documentation.

---

## State Model

Backlog → Drafting → Review → Approved → Ready for Engineering → In Progress → Review → Done

---

## Success Criteria

Every work item follows the same lifecycle, planning and implementation remain separated, engineering starts only from approved specifications, documentation stays synchronized, and every change is traceable.
