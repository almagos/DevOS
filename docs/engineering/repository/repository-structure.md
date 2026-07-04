# Repository Structure

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Entire Repository
>
> This document defines the physical organization of the repository.
>
> It specifies where every class of artifact belongs and which directories are considered canonical.

---

# 1. Purpose

This document defines the repository's physical structure.

Its objectives are to:

- Ensure every artifact has a canonical location.
- Prevent duplicate structures.
- Improve discoverability.
- Keep repository organization consistent.
- Enable predictable navigation for humans and AI.

This document complements `documentation-architecture.md`.

The architecture document explains **why** the repository is organized this way.

This document explains **where** everything belongs.

---

# 2. Repository Layout

```text
/
├── AGENTS.md
├── README.md
├── LICENSE
├── docs/
├── .devos/
├── app/
├── components/
├── lib/
├── public/
├── platform/
├── scripts/
├── supabase/
├── tests/
└── ...
```

The exact application directories may vary by project.

The principles described in this document remain unchanged.

---

# 3. Top-Level Directories

## docs/

Purpose

Canonical repository knowledge.

Characteristics

- Permanent
- Reviewed
- Version-controlled
- Human-authored
- Source of truth

Updated Through

Knowledge Synchronization

---

## .devos/

Purpose

Generated operational state.

Characteristics

- Temporary
- Machine-generated
- Reproducible
- Never manually edited
- Never a source of truth

Updated Through

Automation

---

## app/

Purpose

Application source code.

---

## components/

Purpose

Reusable UI components.

---

## lib/

Purpose

Reusable libraries and utilities.

---

## public/

Purpose

Static assets.

---

## platform/

Purpose

Infrastructure and platform-specific resources.

Examples

- Docker
- Kubernetes
- Infrastructure configuration
- Deployment assets

---

## scripts/

Purpose

Repository automation.

Examples

- Migration scripts
- Maintenance scripts
- Utilities

---

## supabase/

Purpose

Supabase-specific resources.

Examples

- Migrations
- Seed data
- Functions
- Policies

---

## tests/

Purpose

Repository test suites.

---

# 4. Documentation Structure

```text
docs/

├── product/

├── engineering/

├── operations/

├── playbooks/

├── standards/

└── templates/
```

Refer to `documentation-architecture.md` for detailed responsibilities.

---

# 5. Directory Conventions

Every documentation directory should contain a `README.md`.

Directory `README.md` files serve as navigation documents rather than knowledge documents.

Each directory `README.md` should describe:

- Purpose
- What belongs in the directory
- What does not belong in the directory
- Related directories
- Related documentation
- Naming conventions (if applicable)

Directory `README.md` files should not duplicate the contents of the documents within the directory.

Their purpose is to help humans and AI agents navigate the repository consistently.

---

# 6. DevOS Structure

```text
.devos/

└── issues/

    └── <PARENT-ISSUE-ID>/

        ├── context.json

        ├── intent.md

        └── implementation.md
```

Purpose

Generated work packages used by Knowledge Synchronization.

Characteristics

- Generated
- Temporary
- Never manually edited

---

# 7. Artifact Placement Rules

When creating new artifacts:

| Artifact | Location |
|----------|----------|
| Product Feature | docs/product/features/ |
| Product Integration | docs/product/integrations/ |
| Architecture | docs/engineering/architecture/ |
| Pattern | docs/engineering/patterns/ |
| ADR | docs/engineering/decisions/ |
| Runbook | docs/operations/runbooks/ |
| Playbook | docs/playbooks/ |
| Standard | docs/standards/ |
| Template | docs/templates/ |
| Generated Context | .devos/issues/ |

Every artifact has exactly one canonical location.

---

# 8. Repository Ownership

| Directory | Primary Owner |
|------------|---------------|
| docs/ | DevOS |
| .devos/ | Automation |
| app/ | Engineering |
| components/ | Engineering |
| lib/ | Engineering |
| platform/ | Engineering |
| scripts/ | Engineering |
| supabase/ | Engineering |
| tests/ | Engineering |

Ownership defines long-term stewardship.

---

# 9. Repository Rules

- Every directory has a single responsibility.
- Every artifact has one canonical home.
- Repository knowledge belongs under `docs/`.
- Generated operational state belongs under `.devos/`.
- Source code must never become documentation.
- Documentation must never become generated state.
- Avoid creating new top-level directories unless the repository architecture is updated.
- Every documentation directory should contain a `README.md` that serves as its canonical navigation document.

---

# 10. Evolution

The repository structure is expected to remain stable.

Changes should occur only when:

- repeated implementation exposes structural limitations
- repository scale requires evolution
- new knowledge domains emerge

Repository restructuring should be deliberate and infrequent.
