# Issue Context Specification

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Knowledge Synchronization
>
> This document defines the specification for `issue-context.json`.
>
> The Issue Context is the contract between implementation systems and the Knowledge Synchronization workflow.
>
> It provides a complete factual handoff package for a single Parent Issue.

---

# 1. Purpose

The purpose of `issue-context.json` is to provide a complete, self-contained factual representation of a completed Parent Issue.

It enables Knowledge Synchronization without requiring additional lookups into external systems.

The Issue Context is consumed by AI agents to synchronize Canonical Knowledge with implemented reality.

---

# 2. Scope

The Issue Context contains factual information required for Knowledge Synchronization.

Included:

- Parent Issue
- Child Issues
- Pull Requests
- Repository Changes

Excluded:

- Issue comments
- Pull Request comments
- Commit history
- AI-generated summaries
- Documentation updates
- Generated conclusions
- Architectural analysis

Only verified facts are included.

---

# 3. Design Principles

The Issue Context follows the following principles.

## 3.1 Facts Only

The Issue Context contains only verified facts collected from systems of record.

It never contains AI-generated reasoning or conclusions.

---

## 3.2 Self-Contained

The Issue Context provides all information required to perform Knowledge Synchronization.

Knowledge Synchronization should not require additional lookups into Linear or GitHub.

---

## 3.3 Machine Generated

The Issue Context is generated automatically.

It must never be edited manually.

---

## 3.4 Incrementally Updated

The Issue Context is updated after every merged Child Issue Pull Request.

It is never reconstructed from implementation history.

---

## 3.5 One Parent Issue

Each Parent Issue has exactly one Issue Context.

```
.devos/issues/<parent-issue-id>/issue-context.json
```

---

## 3.6 Facts Before Reasoning

Reasoning belongs to Knowledge Synchronization.

The Issue Context only provides facts.

---

# 4. Lifecycle

```
Parent Issue Created
        │
        ▼
Issue Context Created
        │
        ▼
Child PR Merged
        │
        ▼
Append Implementation Facts
        │
        ▼
Repeat Until Parent Complete
        │
        ▼
Knowledge Synchronization
        │
        ▼
Knowledge Sync Report Generated
```

---

# 5. Generation Strategy

The Issue Context is assembled from multiple systems of record.

| Information | Source of Truth |
|-------------|-----------------|
| Parent Issue | Linear |
| Child Issues | Linear |
| Pull Requests | GitHub |
| Changed Files | GitHub |
| Repository Metadata | GitHub Repository |

No information is generated using AI.

---

# 6. Update Strategy

The Issue Context is updated incrementally.

Every merged Child Issue Pull Request appends new implementation facts to the Parent Issue Context.

The Issue Context is never regenerated from historical data.

This avoids expensive reconstruction of implementation history and ensures that the complete implementation context is available when Knowledge Synchronization begins.

---

# 7. Repository Location

Issue Contexts are stored under `.devos`.

```
.devos/

└── issues/

    └── <parent-issue-id>/

        ├── issue-context.json

        └── knowledge-sync-report.md
```

The `.devos` directory contains generated operational state.

It is not Canonical Knowledge.

---

# 8. Source of Truth Model

Different systems own different information.

| Information | Source of Truth |
|-------------|-----------------|
| Parent Issue | Linear |
| Child Issues | Linear |
| Pull Request Details | GitHub |
| Changed Files | GitHub |
| Issue Context | Generated Operational State |
| Canonical Knowledge | Repository Documentation |

The Issue Context is not a source of truth.

It is a generated transport artifact assembled from systems of record.

---

# 9. High-Level Structure

The Issue Context has the following top-level structure.

```
issue-context.json

├── metadata

├── parentIssue

├── childIssues

├── pullRequests

└── repositoryChanges
```

---

# 10. Field Ownership

Every field has exactly one owner.

| Section | Owner |
|----------|-------|
| metadata | Context API |
| parentIssue | Linear |
| childIssues | Linear |
| pullRequests | GitHub |
| repositoryChanges | GitHub |

No field may have multiple owners.

---

# 11. Validation Rules

A valid Issue Context satisfies the following conditions.

- Parent Issue exists.
- Parent Issue is unique.
- Every Child Issue belongs to the Parent Issue.
- Every Pull Request references exactly one Child Issue.
- Every Pull Request includes changed files.
- All information originates from a system of record.
- The Issue Context is machine generated.

---

# 12. Versioning

The Issue Context includes a schema version.

Breaking changes require a schema version increment.

Consumers should validate compatibility before processing an Issue Context.

---

# 13. Future Evolution

Future versions may include additional factual information when required.

Examples include:

- Test execution metadata
- Deployment metadata
- Release metadata

Future versions must continue following the core principles defined in this specification.

Reasoning and generated knowledge should never become part of the Issue Context.
