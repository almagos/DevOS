# Integrations

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** External Integrations
>
> This directory contains integration-specific documentation for DevOS.
>
> Integration documents define how DevOS interacts with external platforms and services.

---

# Purpose

DevOS separates its core architecture from tool-specific implementations.

The core documentation remains tool-agnostic.

Integration documents describe how external systems support the DevOS lifecycle.

---

# Integration Responsibilities

Each integration should define:

- Its purpose
- Its responsibilities
- Its relationship to DevOS
- Applicable standards
- Applicable templates
- Source of Truth ownership

---

# Available Integrations

| Integration | Purpose |
|-------------|---------|
| Linear | Planning and work management |
| GitHub | Source control and implementation |

Additional integrations may be added over time, including automation, deployment, observability, and platform services.

---

# DevOS Lifecycle

```
Planning
        │
        ▼
Linear

↓

Implementation
        │
        ▼
GitHub

↓

Validation

↓

Knowledge Synchronization

↓

Release
```

---

# Design Principles

Integration documentation should:

- Extend DevOS rather than redefine it.
- Reuse repository terminology defined in the Glossary.
- Reference repository documentation rather than duplicate it.
- Remain focused on a single external platform.

---

# Related Documents

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

## Repository Vocabulary

- `docs/glossary.md`
