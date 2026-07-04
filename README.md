# DevOS

> **An AI-Native Development Operating System**
>
> Build software the same way every time—using structured knowledge, standardized workflows, and AI-first engineering.

---

# What is DevOS?

DevOS is an opinionated Development Operating System designed for teams building software with AI.

It treats **knowledge**, **planning**, **implementation**, **validation**, and **documentation** as first-class artifacts rather than disconnected activities.

Instead of relying on undocumented tribal knowledge or prompt engineering, DevOS defines a repeatable operating model that both humans and AI agents can follow consistently.

DevOS is not a framework.

It is not a project management tool.

It is not a coding agent.

It is the operating system that coordinates them.

---

# Why DevOS Exists

Modern AI coding tools can generate code quickly.

What they lack is shared context.

Teams often struggle with:

- Fragmented documentation
- Inconsistent issue quality
- Architecture drift
- Knowledge loss
- Duplicate implementation
- Poor AI context
- Unstructured planning
- Manual documentation

DevOS addresses these problems by making repository knowledge structured, version-controlled and continuously synchronized with implementation.

---

# Core Philosophy

DevOS is built around a few fundamental principles.

## Knowledge First

Knowledge is a first-class artifact.

Documentation is not an afterthought.

---

## One Source of Truth

Every piece of information has exactly one canonical location.

Duplication is treated as technical debt.

---

## AI-Native

Every document is designed to be understandable by both humans and AI agents.

---

## Repository as Knowledge Base

The repository stores implementation knowledge, architecture and operational knowledge—not just source code.

---

## Planning Before Coding

Every implementation begins with structured planning.

---

## Continuous Knowledge Synchronization

Repository knowledge evolves together with implementation.

Documentation reflects implemented reality.

---

# DevOS Architecture

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

---

# Lifecycle

Every feature progresses through the same lifecycle.

```
Ideas

↓

Planning

↓

Implementation

↓

Validation

↓

Knowledge Synchronization

↓

Release

↓

Learning
```

Each stage produces artifacts that become inputs for the next stage.

---

# Core Concepts

| Concept | Purpose |
|---------|---------|
| Repository Constitution | Defines repository governance |
| Glossary | Canonical terminology |
| Contracts | Interfaces between systems |
| Playbooks | Repeatable workflows |
| Standards | Repository rules |
| Templates | Reusable document structures |
| Integrations | External platform conventions |
| Product Knowledge | Business context |
| Engineering Knowledge | Technical implementation |
| Operational Knowledge | Production operation |
| Generated Operational State | Automation artifacts |

---

# Repository Structure

```
.devos/
AGENTS.md
README.md

docs/

    glossary.md

    engineering/

    integrations/

    operations/

    playbooks/

    product/

    standards/

    templates/
```

---

# Technology Independence

DevOS intentionally avoids coupling itself to specific technologies.

Projects may use:

- Next.js
- Flutter
- React
- Laravel
- Go
- Python
- Rust

Likewise, planning and implementation tools may evolve over time.

DevOS currently includes integration guidance for:

- Linear
- GitHub

Additional integrations can be added without changing the core architecture.

---

# AI Workflow

DevOS assumes AI is a first-class engineering participant.

Planning may be performed by humans or AI.

Implementation may be performed by humans or AI.

Validation may be performed by humans or AI.

Knowledge Synchronization may be performed manually or automatically.

The operating model remains the same regardless of who performs each activity.

---

# Source of Truth

| Information | Source of Truth |
|------------|-----------------|
| Planning | Linear |
| Source Code | GitHub |
| Repository Knowledge | Repository Documentation |
| Generated Operational State | `.devos/` |

---

# Design Principles

DevOS follows several architectural principles.

- Knowledge is version controlled.
- Documentation represents implemented reality.
- Every document has exactly one responsibility.
- Every concept has one canonical definition.
- Generated artifacts are never Canonical Knowledge.
- Planning and implementation remain separated.
- External tools are isolated through Integration documentation.
- AI should consume structured context rather than reconstructed context.

---

# Using DevOS

A typical project lifecycle is:

```
Create Repository

↓

Bootstrap DevOS

↓

Define Product

↓

Plan Features

↓

Implement

↓

Validate

↓

Synchronize Knowledge

↓

Release

↓

Repeat
```

---

# Repository Roles

DevOS separates repository responsibilities into distinct domains.

## Product

Defines what is being built.

---

## Engineering

Defines how it is built.

---

## Operations

Defines how it is operated.

---

## Integrations

Defines how external systems participate in the DevOS lifecycle.

---

# Extending DevOS

DevOS is intentionally modular.

Organizations can extend it by adding:

- New Playbooks
- New Standards
- New Templates
- New Integrations
- New Automation

without changing the core operating model.

---

# Versioning

DevOS follows semantic versioning.

Breaking architectural changes should be introduced through new versions rather than modifying historical behavior.

---

# Contributing

Before contributing:

1. Read `AGENTS.md`
2. Read the Documentation Architecture.
3. Read the Repository Structure.
4. Follow the appropriate Playbook.
5. Follow applicable Standards.
6. Use the correct Template.
7. Keep repository knowledge synchronized with implementation.

---

# Roadmap

The long-term vision for DevOS includes:

- Additional platform integrations
- Automated Knowledge Synchronization
- DevOS Upgrade workflows
- Repository health analysis
- Context generation services
- AI-assisted repository governance
- Multi-project DevOS management

---

# License

Choose the license appropriate for your organization.

---

> **DevOS is an operating system for building software—not just writing code.**
