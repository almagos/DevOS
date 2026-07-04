# DevOS Operational State

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Generated Operational State
>
> This directory contains machine-generated operational artifacts used by DevOS.

---

# Purpose

The `.devos/` directory stores generated operational state.

It exists to support workflow automation, AI agents and repository operations.

The contents of this directory are **never** Canonical Knowledge.

---

# Characteristics

Operational State is:

- Machine-generated
- Reproducible
- Temporary
- Automation-friendly

Operational State is not:

- Repository documentation
- Planning
- Source code
- Source of Truth

---

# Typical Contents

Examples include:

```
.devos/

issue-context/

knowledge-sync/

reports/

cache/

metadata/
```

The exact contents may evolve as DevOS automation grows.

---

# Source of Truth

Artifacts stored in this directory should always be reproducible from their authoritative sources.

This directory should never become the primary source of information.

---

# Design Principles

Generated Operational State should:

- Be reproducible.
- Be machine-generated.
- Never require manual editing.
- Never duplicate Canonical Knowledge.
- Support automation rather than documentation.

---

# Relationship to DevOS

```
Planning

↓

Implementation

↓

Validation

↓

Knowledge Synchronization

↓

Generated Operational State
```

Generated Operational State supports repository workflows but is not part of the repository knowledge system.

---

# Related Documents

- `docs/engineering/repository/issue-context-specification.md`
- `docs/engineering/repository/issue-context-model.md`
- `docs/playbooks/knowledge-synchronization.md`
