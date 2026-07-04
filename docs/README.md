# Documentation

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> Welcome to the canonical documentation for this repository.
>
> The repository follows a knowledge-first documentation architecture where documentation is treated as a first-class artifact and remains synchronized with implemented reality.

---

# Quick Start

Choose the path that best matches your role.

## AI Agent

Read in the following order:

1. `/AGENTS.md`
2. `engineering/repository/documentation-architecture.md`
3. `engineering/repository/repository-structure.md`
4. Relevant Playbook
5. Relevant Standards
6. Relevant Template
7. Domain Documentation
8. Assigned Task

---

## Product

Start here:

```
product/
├── strategy/
├── domain/
├── users/
├── features/
└── integrations/
```

---

## Engineering

Start here:

```
engineering/
├── architecture/
├── platform/
├── repository/
├── patterns/
└── decisions/
```

---

## Operations

Start here:

```
operations/
├── release/
├── monitoring/
└── runbooks/
```

---

# Documentation Map

```
docs/

├── product/
│   What are we building?
│
├── engineering/
│   How is it built?
│
├── operations/
│   How is it operated?
│
├── playbooks/
│   How is work performed?
│
├── standards/
│   What rules govern the repository?
│
└── templates/
    How should recurring documents be structured?
```

---

# Documentation Domains

## Product

Defines the product from a business perspective.

Examples:

- Vision
- Principles
- Domain
- Users
- Features
- Product Integrations

---

## Engineering

Defines the technical implementation.

Examples:

- Architecture
- Platform
- Repository
- Patterns
- Architecture Decisions

---

## Operations

Defines how the system is operated.

Examples:

- Release
- Monitoring
- Runbooks

---

## Playbooks

Defines repeatable workflows.

Examples:

- Planning
- Implementation
- Validation
- Knowledge Synchronization
- Release
- Maintenance

---

## Standards

Defines repository rules and conventions.

Examples:

- Documentation
- Repository
- Naming
- Writing
- Diagrams

---

## Templates

Provides reusable document templates.

Examples:

- Feature
- Integration
- Architecture
- Pattern
- ADR
- Playbook
- Runbook

---

# Repository Constitution

The repository is governed by the following constitutional documents.

1. `/AGENTS.md`
2. `engineering/repository/documentation-architecture.md`
3. `engineering/repository/repository-structure.md`

These documents define how the repository is organized and should be consulted before introducing structural changes.

---

# Repository Principles

The documentation system follows these principles.

- Canonical Knowledge is a first-class artifact.
- Every document has exactly one canonical home.
- Documentation reflects implemented reality.
- Generated operational state is never a source of truth.
- Repeatable workflows are defined by playbooks.
- Repository rules are defined by standards.
- Recurring documents use templates.

---

# Contributing Documentation

Before creating or modifying documentation:

1. Read the relevant playbook.
2. Follow applicable standards.
3. Use the appropriate template.
4. Update Canonical Knowledge through the Knowledge Synchronization workflow.

Avoid introducing duplicate knowledge or undocumented repository structure.

---

# Related Documents

Repository Constitution

- `engineering/repository/documentation-architecture.md`
- `engineering/repository/repository-structure.md`

Repository Bootstrap

- `/AGENTS.md`

Documentation Framework

- `playbooks/`
- `standards/`
- `templates/`

Documentation Domains

- `product/`
- `engineering/`
- `operations/`
