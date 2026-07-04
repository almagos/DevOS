# Commit Standard

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** GitHub Integration
>
> This standard defines how commits are created within DevOS.
>
> All commits must comply with this standard.

---

# 1. Purpose

This standard defines the conventions for creating Git commits within DevOS.

Commits represent implementation history.

They should be:

- Atomic
- Reviewable
- Traceable
- Reversible

Commits are implementation artifacts.

They are not planning artifacts or repository documentation.

---

# 2. Scope

This standard applies to:

- Human contributors
- AI agents
- Automation

It governs every commit created within the repository.

---

# 3. Commit Principles

Every commit should:

- Represent one logical implementation step.
- Be independently understandable.
- Leave the repository in a working state.
- Be reversible whenever practical.
- Contribute toward exactly one Child Issue.

Commits should never combine unrelated work.

---

# 4. Commit Message Format

Use the following format.

```
<type>: <short description>
```

Examples:

```
feat: implement portfolio import validation

fix: handle empty transaction history

docs: update repository structure

refactor: simplify context generation

test: add validation workflow tests

chore: update development dependencies
```

---

# 5. Commit Types

| Type | Purpose |
|------|---------|
| feat | New functionality |
| fix | Bug fix |
| docs | Documentation |
| refactor | Internal improvement |
| test | Tests |
| chore | Repository maintenance |
| perf | Performance improvement |
| build | Build or dependency changes |
| ci | Continuous Integration |
| revert | Revert previous commit |

---

# 6. Commit Rules

Commits should:

- Be small.
- Build successfully.
- Pass applicable validation.
- Avoid unrelated formatting changes.
- Avoid unrelated refactoring.
- Avoid generated artifacts unless intentionally version controlled.

---

# 7. Relationship to Child Issues

A Child Issue may contain multiple commits.

However:

- Every commit should contribute toward only one Child Issue.
- Commits should not span multiple Child Issues.
- The Pull Request represents the completed Child Issue.

---

# 8. Things to Avoid

Do not create commits that:

- Mix unrelated features.
- Include unfinished experiments.
- Contain temporary debugging code.
- Include commented-out implementations.
- Introduce unrelated formatting changes.
- Bundle documentation updates unrelated to the implementation.

---

# 9. Validation

Before committing, verify:

- Repository builds successfully.
- Relevant tests pass.
- Commit message follows this standard.
- No unrelated files are included.

---

# 10. Related Documents

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

---

## Related Playbooks

- `docs/playbooks/implementation.md`
- `docs/playbooks/validation.md`

---

## Related Standards

- `pull-request-standard.md`

---

## Related Templates

- `pull-request-template.md`
