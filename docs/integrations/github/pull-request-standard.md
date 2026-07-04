# Pull Request Standard

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** GitHub Integration
>
> This standard defines how Pull Requests are created and reviewed within DevOS.
>
> All Pull Requests must comply with this standard.

---

# 1. Purpose

This standard defines the conventions governing Pull Requests within DevOS.

A Pull Request represents the completion of one Child Issue.

It provides the implementation, validation evidence, and review required before merging into the repository.

Pull Requests are implementation artifacts.

They are not planning artifacts or Canonical Knowledge.

---

# 2. Scope

This standard applies to:

- Human contributors
- AI agents
- Automation

It governs every Pull Request created within the repository.

---

# 3. Pull Request Principles

Every Pull Request should:

- Implement exactly one Child Issue.
- Be independently reviewable.
- Remain focused on one objective.
- Include all implementation required to satisfy the Child Issue.
- Leave the repository in a working state.

Large Parent Issues should be implemented through multiple Pull Requests rather than one large Pull Request.

---

# 4. Pull Request Title

Use the following format.

```
<Child Issue Title>
```

Examples:

```
Implement portfolio import validation

Add issue context generation

Create repository documentation index
```

The Pull Request title should match the corresponding Child Issue title.

---

# 5. Pull Request Requirements

Every Pull Request should include:

- Summary of implementation
- Scope of changes
- Validation performed
- Related Child Issue
- Related Parent Issue
- Known limitations (if any)

---

# 6. Relationship to DevOS

A Pull Request represents:

```
Planning

↓

Implementation

↓

Validation

↓

Ready for Knowledge Synchronization
```

A Pull Request does not update Canonical Knowledge directly.

Knowledge Synchronization occurs after the Pull Request has been validated and merged.

---

# 7. Review Rules

Review should verify:

- Scope matches the Child Issue.
- Acceptance Criteria have been satisfied.
- Repository standards have been followed.
- Implementation aligns with approved architecture.
- No unrelated work has been introduced.

Review should focus on implementation quality rather than redesigning approved planning.

---

# 8. Merge Requirements

A Pull Request should only be merged when:

- Required reviews have completed.
- Validation has passed.
- Repository builds successfully.
- Acceptance Criteria have been satisfied.
- The implementation is ready for Knowledge Synchronization.

---

# 9. Things to Avoid

Do not create Pull Requests that:

- Implement multiple Child Issues.
- Mix unrelated work.
- Introduce undocumented architectural changes.
- Include temporary debugging code.
- Contain unrelated formatting or refactoring.

---

# 10. Related Documents

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

---

## Repository Vocabulary

- `docs/glossary.md`

---

## Related Playbooks

- `docs/playbooks/implementation.md`
- `docs/playbooks/validation.md`
- `docs/playbooks/knowledge-synchronization.md`

---

## Related Standards

- `commit-standard.md`

---

## Related Templates

- `pull-request-template.md`
