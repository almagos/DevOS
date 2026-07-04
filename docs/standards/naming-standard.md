# Naming Standard

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Repository Naming
>
> This standard defines the naming conventions used throughout the repository.
>
> Consistent naming improves discoverability, maintainability, and AI navigation.

---

# 1. Purpose

The purpose of this standard is to ensure repository names are:

- Consistent
- Predictable
- Discoverable
- Unambiguous
- AI-friendly

Naming is considered part of repository architecture.

---

# 2. Scope

This standard applies to:

- Directories
- Documentation
- Playbooks
- Standards
- Templates
- Runbooks
- Architecture documents

It does not prescribe naming conventions for source code.

---

# 3. Naming Principles

All repository names follow these principles.

## Principle 1

Names should describe purpose rather than implementation.

---

## Principle 2

Names should remain stable over time.

---

## Principle 3

Names should be unambiguous.

---

## Principle 4

The same concept should always use the same name.

---

## Principle 5

Prefer explicit names over abbreviated names.

---

# 4. File Naming

Documentation files use:

- lowercase
- words separated by hyphens
- descriptive names

Examples:

```
documentation-architecture.md

repository-structure.md

issue-context-specification.md

issue-context-model.md

knowledge-synchronization.md
```

Avoid:

```
architecture.md

repo.md

context.md

sync.md
```

---

# 5. Directory Naming

Directories use:

- lowercase
- singular or plural based on responsibility
- descriptive names

Examples:

```
product/

engineering/

operations/

playbooks/

standards/

templates/
```

---

# 6. Document Naming

Document names should describe their responsibility.

Examples:

```
documentation-standard.md

repository-standard.md

writing-standard.md

naming-standard.md
```

Avoid generic names.

---

# 7. Terminology

Repository terminology should remain consistent.

Examples include:

- Parent Issue
- Child Issue
- Canonical Knowledge
- Knowledge Synchronization
- Repository Constitution
- Generated Operational State

Repository terminology should not be redefined without updating the Glossary.

---

# 8. Compliance

Repository naming complies with this standard when:

- Names are descriptive.
- Naming conventions are followed.
- Repository terminology remains consistent.

---

# 9. Exceptions

Exceptions should be rare.

They should improve clarity rather than reduce consistency.

---

# 10. Related Documents

## Repository Constitution

- AGENTS.md
- Documentation Architecture
- Repository Structure

## Related Standards

- Documentation Standard
- Repository Standard
- Writing Standard

## Related Playbooks

- Planning
- Implementation
- Validation
- Knowledge Synchronization
- Release
