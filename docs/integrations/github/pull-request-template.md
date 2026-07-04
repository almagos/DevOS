# Pull Request Template

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** GitHub Integration
>
> This template defines the canonical structure for Pull Request descriptions within DevOS.
>
> Every Pull Request should follow this structure.

---

# Purpose

This template standardizes Pull Request descriptions to improve review quality, implementation traceability and Knowledge Synchronization.

A Pull Request represents the completed implementation of exactly one Child Issue.

---

# Related Child Issue

Reference the Child Issue implemented by this Pull Request.

Example:

```
ALM-123
```

---

# Related Parent Issue

Reference the Parent Issue.

Example:

```
ALM-45
```

---

# Summary

Describe what was implemented.

Focus on the outcome rather than individual commits.

---

# Scope

Summarize the implemented changes.

Examples:

- New functionality
- Bug fixes
- UI changes
- API changes
- Database changes
- Tests
- Documentation

---

# Repository Impact

Describe the repository areas affected.

Examples:

- Pages
- Components
- Routes
- APIs
- Database
- Storage
- Configuration
- Documentation

---

# Validation

Summarize validation performed.

Examples:

- Manual testing
- Automated tests
- Mobile testing
- Cross-browser testing
- Performance validation
- Security validation

---

# Acceptance Criteria

Summarize how the Child Issue acceptance criteria have been satisfied.

---

# Known Limitations

List any remaining limitations that are intentionally deferred.

If none, state:

```
None.
```

---

# Knowledge Synchronization

Identify the repository documentation expected to change after merge.

Examples:

- Architecture
- Repository documentation
- Standards
- Patterns
- Runbooks

If no documentation updates are expected, state:

```
No repository documentation changes required.
```

---

# Checklist

- [ ] Implements exactly one Child Issue.
- [ ] Acceptance Criteria satisfied.
- [ ] Validation completed.
- [ ] Repository builds successfully.
- [ ] No unrelated changes included.
- [ ] Ready for review.
- [ ] Ready for Knowledge Synchronization.

---

# Related Documents

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

- `docs/integrations/github/pull-request-standard.md`
- `docs/integrations/github/commit-standard.md`
