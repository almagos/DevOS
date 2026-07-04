# DevOS Documentation Index

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Entire Repository
>
> This document provides the primary entry point into the DevOS documentation system.
>
> It explains how repository knowledge is organized and how contributors—human or AI—should navigate it.

---

# Documentation Architecture

Repository knowledge is organized into three architectural layers.

```
Core DevOS
│
├── Repository Constitution
├── Glossary
├── Contracts
├── Playbooks
├── Standards
├── Templates
└── Integrations

↓

Project Knowledge
│
├── Product
├── Engineering
└── Operations

↓

Generated Operational State
│
└── .devos/
```

Each layer has a distinct responsibility.

- **Core DevOS** defines how work is planned, implemented, validated and documented.
- **Project Knowledge** describes the implemented product and its operation.
- **Generated Operational State** supports automation and AI workflows and is never Canonical Knowledge.

---

# Reading Order

New contributors should read documentation in the following order.

| Level | Documents                                                                     |
| ----- | ----------------------------------------------------------------------------- |
| 0     | `AGENTS.md`                                                                   |
| 1     | Documentation Architecture<br>Repository Structure                            |
| 2     | Glossary                                                                      |
| 3     | Relevant Playbooks                                                            |
| 4     | Relevant Standards                                                            |
| 5     | Relevant Templates                                                            |
| 6     | Relevant Integration Documentation *(when interacting with external systems)* |
| 7     | Domain Documentation                                                          |
| 8     | Assigned Task                                                                 |


---

# Documentation Map

## Repository Constitution

Defines the repository foundation.

| Document | Purpose |
|----------|---------|
| `AGENTS.md` | Repository operating instructions |
| `engineering/repository/documentation-architecture.md` | Documentation architecture |
| `engineering/repository/repository-structure.md` | Repository architecture |

---

## Glossary

Defines the canonical repository vocabulary.

| Document | Purpose |
|----------|---------|
| `glossary.md` | Canonical terminology |

---

## Contracts

Define interfaces between repository systems.

| Document | Purpose |
|----------|---------|
| `engineering/repository/issue-context-specification.md` | Issue Context contract |
| `engineering/repository/issue-context-model.md` | Issue Context data model |

---

## Playbooks

Define lifecycle workflows.

| Document | Purpose |
|----------|---------|
| `planning.md` | Planning workflow |
| `implementation.md` | Implementation workflow |
| `validation.md` | Validation workflow |
| `knowledge-synchronization.md` | Knowledge Synchronization workflow |
| `release.md` | Release workflow |

---

## Standards

Define repository rules.

| Document | Purpose |
|----------|---------|
| `documentation-standard.md` | Documentation rules |
| `repository-standard.md` | Repository organization rules |
| `writing-standard.md` | Writing conventions |
| `naming-standard.md` | Naming conventions |

---

## Templates

Provide reusable document structures.

| Document | Purpose |
|----------|---------|
| `adr-template.md` | Architectural Decision Records |
| `playbook-template.md` | Playbooks |
| `standard-template.md` | Standards |
| `architecture-document-template.md` | Architecture documents |
| `runbook-template.md` | Runbooks |

---

## Integrations

Define how DevOS interacts with external platforms.

| Document | Purpose |
|----------|---------|
| `integrations/README.md` | Integration architecture |
| `integrations/linear/` | Planning integration |
| `integrations/github/` | Implementation integration |

---

## Domain Knowledge

Project-specific knowledge is organized by domain.

```
docs/

├── product/
│   What are we building?
│
├── engineering/
│   How is it built?
│
└── operations/
    How is it operated?
```

---

## Generated Operational State

Machine-generated operational artifacts are stored under:

```
.devos/
```

Examples include:

- Issue Context
- Knowledge Synchronization Reports
- Generated Metadata

Generated Operational State is reproducible and is never Canonical Knowledge.

---

# Source of Truth

Every category of information has exactly one Source of Truth.

| Information | Source of Truth |
|-------------|-----------------|
| Planning | Project Management System |
| Source Code | Version Control |
| Canonical Knowledge | `docs/` |
| Generated Operational State | `.devos/` |

---

# Repository Principles

The repository follows these principles.

- Every document has exactly one responsibility.
- Every piece of knowledge has exactly one canonical location.
- Documentation represents implemented reality.
- Generated Operational State is never Canonical Knowledge.
- Stable terminology is defined by the Glossary.
- Repository workflows are defined by Playbooks.
- Repository rules are defined by Standards.
- Recurring document structures are defined by Templates.
- External platforms are governed by Integration documentation.

---

# Contributing Documentation

Before creating or modifying documentation:

1. Read the relevant playbook.
2. Review applicable standards.
3. Use the appropriate template.
4. Update Canonical Knowledge through the Knowledge Synchronization workflow.

Avoid:

- Duplicate knowledge
- Undocumented repository structure
- Inconsistent terminology
- Manual updates outside the appropriate workflow

---

# Related Documents

## Repository Constitution

- `AGENTS.md`
- `engineering/repository/documentation-architecture.md`
- `engineering/repository/repository-structure.md`

---

## Repository Vocabulary

- `glossary.md`

---

## Repository Framework

- `playbooks/`
- `standards/`
- `templates/`

---

## Integrations

- `integrations/`
- `integrations/linear/`
- `integrations/github/`

---

## Domain Knowledge

- `product/`
- `engineering/`
- `operations/`
