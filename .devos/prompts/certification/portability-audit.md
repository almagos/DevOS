# Repository Portability Audit Prompt

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Compatible Agents:** ChatGPT, Claude, Codex, Antigravity
>
> **Related Playbook:** `docs/playbooks/bootstrap-certification.md`
>
> **Related Standard:** `docs/standards/repository-standard.md`

---

# Purpose

This prompt evaluates whether a repository is fully portable and suitable for distribution as a GitHub Template Repository.

The audit verifies that repository documentation, navigation and structure remain independent of local environments, historical repository names and obsolete references.

The prompt performs validation only.

It may apply mechanical repairs when explicitly requested.

---

# Prerequisites

Before executing this prompt ensure that:

- Repository documentation has been committed.
- Repository restructuring has been completed.
- Internal documentation links are expected to be stable.

---

# Inputs

Repository root.

Repository documentation.

Repository directory structure.

---

# Prompt

Perform a complete Repository Portability Audit.

## Objective

Determine whether this repository is fully portable and suitable for use as a reusable GitHub Template Repository.

Search the entire repository for portability issues.

Do not redesign the repository architecture.

Only repair portability-related issues when instructed.

---

## Validation Requirements

Search the repository for:

- Absolute filesystem paths
- Legacy repository names
- Broken Markdown links
- Incorrect relative links
- References to deleted documents
- References to moved documents
- Broken README navigation
- Undocumented top-level files

Validate every internal Markdown link.

Verify that every referenced document exists.

Verify that every README correctly navigates its directory.

Verify that repository navigation remains deterministic.

---

## Repository Branding

Identify unintended references to:

- Previous repository names
- Local development environments
- Historical extraction artifacts

Do not remove intentional historical documentation.

---

## Relative Link Policy

Repository documentation should use relative Markdown links for internal navigation whenever practical.

Do not rewrite legitimate external URLs.

---

## Validation

Confirm:

- No broken internal links.
- No absolute filesystem paths.
- No obsolete internal references.
- No undocumented repository artifacts.
- Consistent repository navigation.

---

## Report

Produce a Portability Audit Report containing:

- Files Modified (if applicable)
- Issues Found
- Issues Fixed
- Remaining Issues
- Validation Summary
- Repository Portability Status

---

## Constraints

Do not redesign repository architecture.

Do not rewrite documentation unnecessarily.

Prefer the smallest possible mechanical change.

---

# Deliverables

Produce a Portability Audit Report.

If repair mode is enabled, apply only mechanical portability fixes.

---

# Success Criteria

The audit succeeds when:

- Internal documentation links resolve successfully.
- Repository navigation remains deterministic.
- No local filesystem references remain.
- Repository documentation is portable across environments.
- The repository is suitable for publication as a GitHub Template Repository.

---

# Related Documentation

## Standards

- `docs/standards/repository-standard.md`

## Playbooks

- `docs/playbooks/bootstrap-certification.md`

## Repository Constitution

- `AGENTS.md`
