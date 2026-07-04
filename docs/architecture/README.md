
# Architecture

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Repository Architecture
>
> This directory contains the high-level architectural description of the repository and the systems built using DevOS.

---

# Purpose

Architecture documents explain the fundamental design of the system.

They answer **why the system exists**, **what it is**, **who it serves**, and **how it works**.

Architecture documents describe stable concepts rather than implementation details.

---

# Architecture Framework

DevOS organizes architecture into four complementary perspectives.

| Document | Purpose |
|----------|---------|
| `why.md` | Why the system exists |
| `what.md` | What the system is |
| `who.md` | Who the stakeholders and users are |
| `how.md` | How the system is designed and operates |

Together these documents provide a complete architectural understanding of the system.

---

# Design Principles

Architecture documents should:

- Describe stable concepts.
- Focus on long-term design.
- Remain implementation independent where possible.
- Explain decisions rather than implementation.
- Reference detailed documentation instead of duplicating it.

Architecture documentation should evolve slowly.

---

# Relationship to DevOS

Architecture documents provide the conceptual foundation for all other repository knowledge.

```
Why

↓

What

↓

Who

↓

How

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
```

Planning and implementation should align with the architecture defined in this directory.

---

# What Belongs Here

Examples include:

- Vision
- Mission
- System Architecture
- Architectural Principles
- Stakeholders
- Domain Overview
- High-Level Design
- Architectural Constraints

---

# What Does Not Belong Here

Do not include:

- Feature specifications
- Implementation details
- Coding patterns
- Repository standards
- Operational procedures
- Temporary design discussions
- Implementation history

These belong elsewhere in the repository.

---

# Related Documents

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

---

## Related Documentation

- `docs/product/`
- `docs/engineering/`
- `docs/operations/`

---

## Related Standards

- `docs/standards/documentation-standard.md`
- `docs/standards/writing-standard.md`
