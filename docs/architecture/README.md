# Architecture

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Repository Architecture
>
> This directory contains architecture documentation that describes the stable design of a repository or system built using DevOS.

---

# Purpose

Architecture documents explain the long-term structure of a system.

They describe:

- Why the architecture exists.
- The major architectural concepts.
- High-level system design.
- Stable boundaries and responsibilities.
- Significant architectural constraints.

Architecture documentation should remain stable over time and avoid implementation-specific details.

---

# What Belongs Here

Examples include:

- System Architecture
- Repository Architecture
- Platform Architecture
- Integration Architecture
- Data Architecture
- Security Architecture
- Deployment Architecture
- Architectural Principles
- High-Level Design

Not every repository requires every architecture document.

Only create architecture documents that provide long-term value.

---

# What Does Not Belong Here

Do not place the following in this directory:

- Feature specifications
- User requirements
- Coding standards
- Implementation details
- Playbooks
- Runbooks
- Temporary design discussions
- Meeting notes

These belong in their respective repository domains.

---

# Design Principles

Architecture documentation should:

- Describe stable concepts.
- Explain structure rather than implementation.
- Focus on long-term maintainability.
- Reference detailed documentation instead of duplicating it.
- Remain implementation independent whenever practical.

Architecture should evolve slowly compared to implementation.

---

# Relationship to DevOS

Architecture provides the foundation for repository knowledge.

```
Architecture

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

Architectural decisions guide implementation and should remain consistent with the repository standards.

---

# Related Documents

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

---

## Related Documentation

- `docs/playbooks/`
- `docs/standards/`
- `docs/templates/`

---

## Related Templates

- `docs/templates/architecture-document-template.md`

---

## Related Standards

- `docs/standards/documentation-standard.md`
- `docs/standards/writing-standard.md`
