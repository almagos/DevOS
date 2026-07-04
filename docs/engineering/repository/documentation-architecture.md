# Documentation Architecture

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Entire Repository
>
> This document defines the documentation architecture used by this repository.
>
> It is the authoritative specification for how knowledge is organized, maintained, and evolved throughout the software lifecycle.
>
> All contributors—human or AI—must follow this architecture.

---

# 1. Purpose

The purpose of this architecture is to ensure that repository knowledge remains:

- Accurate
- Discoverable
- Maintainable
- AI-friendly
- Free from duplication
- Free from documentation drift

The repository is treated as the canonical source of implemented knowledge.

Planning and implementation occur outside the repository. Only validated, implemented knowledge becomes permanent documentation.

---

# 2. Non-Goals

This repository intentionally does **not** serve the following purposes.

## 2.1 Planning System

Planning belongs in the project management system.

Examples include:

- Ideas
- Feature proposals
- Roadmaps
- Prioritization
- Implementation planning

Planning information should not become permanent repository documentation until it has been implemented.

---

## 2.2 Implementation History

Implementation history belongs in version control.

Examples include:

- Commits
- Pull requests
- Code reviews
- Implementation discussions

Repository documentation captures implemented knowledge rather than implementation history.

---

## 2.3 Discussion Archive

Repository documentation is not intended to preserve brainstorming, design exploration, or intermediate discussions.

Only validated decisions that become implemented knowledge should be documented.

---

## 2.4 Generated Operational State

Generated artifacts are not documentation.

Examples include:

- Issue Context Packages
- Generated reports
- Temporary AI outputs
- Synchronization state

Generated operational artifacts belong under `.devos/`.

---

## 2.5 Duplicate Knowledge

Every piece of knowledge must have exactly one canonical location.

Cross-references are encouraged.

Duplication is not.

---

## 2.6 AI Memory

The repository is not intended to become an AI conversation log.

Reasoning, exploration, and intermediate thinking should remain outside the repository unless they result in implemented knowledge.

---

# 3. Design Principles

This documentation architecture is built on the following principles.

## 3.1 Knowledge First

Knowledge is treated as a first-class artifact.

Documentation is not an afterthought.

Implementation is expected to update repository knowledge through the Knowledge Synchronization workflow.

---

## 3.2 One Source of Truth

Every piece of knowledge has exactly one canonical location.

Information must never be duplicated across documents.

Documents may reference each other but should not copy content.

---

## 3.3 Stable Knowledge Only

The repository stores stable knowledge.

It does not store:

- Planning discussions
- Brainstorming
- Temporary decisions
- Implementation notes
- Generated context

Those belong to their respective systems.

---

## 3.4 Separation of Concerns

Documentation is organized by knowledge domain.

Each domain answers a different question.

| Domain | Question |
|----------|----------|
| Product | What are we building? |
| Engineering | How is it built? |
| Operations | How is it operated? |
| Playbooks | How is work performed? |
| Standards | What rules govern documentation? |
| Templates | How should recurring documents begin? |

---

## 3.5 AI Native

The documentation architecture is designed for both humans and AI agents.

Every document should be:

- Predictable
- Discoverable
- Self-contained
- Machine-readable
- Cross-referenced

---

# 4. Repository Philosophy

The repository represents implemented reality.

It is **not** the planning system.

It is **not** the work tracking system.

It is **not** the implementation history.

Those responsibilities belong elsewhere.

| Information | Source of Truth |
|-------------|-----------------|
| Planned Work | Project Management System |
| Source Code | Version Control |
| Implemented Knowledge | Repository Documentation |
| Generated Operational State | `.devos/` |

---

# 5. Documentation Domains

```
docs/

product/
engineering/
operations/
playbooks/
standards/
templates/
```

Each top-level directory represents a stable knowledge domain.

---

## Product

Purpose

Describe what the product is.

Contains:

- Strategy
- Domain
- Users
- Features
- Product Integrations

---

## Engineering

Purpose

Describe how the system is implemented.

Contains:

- Architecture
- Platform
- Repository
- Patterns
- Architecture Decisions

---

## Operations

Purpose

Describe how the system is operated.

Contains:

- Release
- Monitoring
- Runbooks

---

## Playbooks

Purpose

Describe repeatable workflows.

Playbooks are workflow-oriented rather than agent-oriented.

They define processes independently of the tools or AI agents executing them.

---

## Standards

Purpose

Define repository standards.

Standards define constraints and conventions.

They do not define workflows.

---

## Templates

Purpose

Provide reusable starting points for recurring document types.

Templates improve consistency across documentation.

---

# 6. Documentation Lifecycle

Knowledge progresses through several stages.

```
Idea

↓

Planning

↓

Implementation

↓

Validation

↓

Knowledge Synchronization

↓

Repository Documentation
```

Documentation is updated only after implementation has been validated.

---

# 7. Source of Truth Model

Different systems own different kinds of information.

| Information | Source of Truth |
|-------------|-----------------|
| Planning | Project Management System |
| Implementation | Version Control |
| Repository Knowledge | Documentation |
| Operational State | `.devos/` |

Repository documentation should never duplicate planning information or implementation history.

---

# 8. Knowledge Ownership

Knowledge ownership is determined by domain.

| Domain | Primary Owner |
|----------|---------------|
| Product | Product Planning |
| Engineering | Engineering |
| Operations | Engineering / DevOps |
| Playbooks | DevOS |
| Standards | DevOS |
| Templates | DevOS |

Ownership determines long-term stewardship rather than who edits a document on a given day.

---

# 9. Knowledge Synchronization

Repository documentation is updated through the Knowledge Synchronization workflow.

Knowledge Synchronization is responsible for:

- Identifying affected documentation
- Updating canonical knowledge
- Removing obsolete information
- Maintaining repository consistency

Documentation should never be manually updated during implementation unless explicitly required by a playbook.

---

# 10. Repository Laws

The following rules are considered invariant.

## Law 1

Every document has exactly one canonical home.

---

## Law 2

The repository documents implemented reality.

---

## Law 3

Planning belongs outside the repository.

---

## Law 4

Generated artifacts never become sources of truth.

---

## Law 5

Every recurring document type has a template.

---

## Law 6

Every repeatable workflow has a playbook.

---

## Law 7

Documentation must remain synchronized with implementation.

---

# 11. Relationship with DevOS

The repository contains two distinct kinds of information.

## Canonical Knowledge

Located under:

```
docs/
```

Characteristics:

- Permanent
- Reviewed
- Version-controlled
- Human-authored
- Source of truth

---

## Operational State

Located under:

```
.devos/
```

Characteristics:

- Generated
- Temporary
- Reproducible
- Machine-generated
- Never manually edited
- Never a source of truth

---

# 12. Evolution

This architecture is intended to remain stable.

Changes should occur only when:

- Repeated implementation experience exposes structural problems
- Repository scale requires architectural evolution
- New knowledge domains emerge

Repository restructuring should be rare.

Stability is preferred over continual optimization.
