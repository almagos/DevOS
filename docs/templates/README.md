# Templates

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Repository Templates
>
> This directory contains the canonical templates for recurring documentation artifacts within DevOS.
>
> Templates define document structure. They do not define repository rules or workflows.

---

# Purpose

Templates provide standardized structures for recurring documentation.

They promote consistency across the repository while reducing duplication and ensuring both humans and AI agents produce documentation with a common format.

Templates define **how documents are structured**, not **what they should contain**.

---

# Contains

Examples include:

- ADR Templates
- Architecture Document Templates
- Certification Report Templates
- Playbook Templates
- Runbook Templates
- Specification Templates
- Standard Templates

---

# Does Not Contain

This directory does not contain:

- Completed documentation
- Repository standards
- Repository workflows
- Project-specific knowledge
- Generated operational artifacts

---

# Relationship to DevOS

Templates are used throughout the repository lifecycle.

```
Playbooks

↓

Standards

↓

Templates

↓

Repository Documents
```

Playbooks describe **when** documentation is created.

Standards describe **how** documentation should be written.

Templates define **how** recurring documents should be structured.

---

# Naming Convention

Template files use lower-case kebab-case with the `-template` suffix.

Examples:

- `adr-template.md`
- `architecture-document-template.md`
- `certification-report-template.md`
- `playbook-template.md`
- `runbook-template.md`
- `specification-template.md`
- `standard-template.md`

---

# Related Directories

- `docs/playbooks/`
- `docs/standards/`

---

# Related Documents

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

---

## Related Standards

- `docs/standards/documentation-standard.md`
- `docs/standards/writing-standard.md`

---

## Related Playbooks

- `docs/playbooks/planning.md`
- `docs/playbooks/implementation.md`
- `docs/playbooks/knowledge-synchronization.md`
