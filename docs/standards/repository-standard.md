# Repository Standard

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Repository Structure
>
> This standard defines the structural rules governing the repository.
>
> All repository content must comply with this standard.

---

# 1. Purpose

The purpose of this standard is to ensure the repository remains:

- Predictable
- Discoverable
- Maintainable
- Scalable
- AI-friendly

Repository organization is considered a long-term architectural concern.

---

# 2. Scope

This standard applies to the entire repository.

It governs:

- Directory structure
- File placement
- Knowledge organization
- Generated artifacts

---

# 3. Repository Principles

All repository content follows these principles.

## Principle 1

Every artifact has exactly one canonical location.

---

## Principle 2

Repository structure follows knowledge domains rather than teams, tools, or technologies.

---

## Principle 3

Generated operational artifacts must remain separate from Canonical Knowledge.

---

## Principle 4

Repository organization should remain stable over time.

Structural changes should be rare.

---

## Principle 5

Repository navigation should be predictable for both humans and AI agents.

---

# 4. Top-Level Directories

Each top-level directory has a single architectural responsibility.

| Directory | Purpose |
|-----------|---------|
| `docs/` | Canonical Knowledge |
| `.devos/` | Generated Operational State |
| `.github/` | Repository automation and GitHub configuration |
| `apps/` | Applications and deployable services |
| `packages/` | Shared libraries and reusable modules |
| `platform/` | Platform-specific infrastructure and configuration (for example `supabase/`, `vercel/`, `cloudflare/`) |
| `scripts/` | Repository automation and developer tooling |

Repository standards define architectural responsibilities rather than framework- or platform-specific directory names.

Individual projects may organize implementation differently provided they preserve the responsibilities defined by this standard.

Additional top-level directories should be introduced only when they represent a distinct architectural responsibility.

Every top-level directory must have exactly one clearly defined purpose.

Top-level responsibilities must not overlap.

---

# 5. Documentation Placement

Repository documentation must follow the Documentation Architecture.

Each document must be stored in its canonical location.

Documents must not be duplicated across multiple directories.

---

# 6. Generated Artifacts

Generated operational artifacts belong under:

```
.devos/
```

Examples include:

- Issue Context
- Knowledge Synchronization Reports
- Generated metadata
- Machine-generated state

Generated artifacts are never Canonical Knowledge.

---

# 7. Repository Evolution

Repository structure should evolve conservatively.

New directories should be introduced only when:

- Existing domains cannot reasonably accommodate new knowledge.
- A distinct architectural responsibility emerges.

---

# 8. Directory Ownership

Each directory has one primary responsibility.

Directories should not overlap in purpose.

---

# 9. Compliance

The repository is compliant when:

- Repository Structure is followed.
- Documentation Architecture is followed.
- Repository Standards are satisfied.
- Canonical Knowledge remains organized by domain.

---

# 10. Exceptions

Exceptions should be rare.

Any exception must:

- Be justified.
- Preserve repository consistency.
- Avoid introducing duplicate structure.

---

# 11. Related Documents

## Repository Constitution

- AGENTS.md
- Documentation Architecture
- Repository Structure

## Related Standards

- Documentation Standard
- Naming Standard
- Writing Standard

## Related Playbooks

- Knowledge Synchronization
