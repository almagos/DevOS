# Issue Context Model

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Issue Context
>
> This document defines the logical data model for `issue-context.json`.
>
> The model defines the structure, ownership, and semantics of every field contained within an Issue Context.

---

# 1. Purpose

The Issue Context Model defines the complete factual representation of a Parent Issue.

It serves as the data contract between:

- Project Management
- Version Control
- Context API
- Knowledge Synchronization

The model is implementation independent.

Although currently serialized as JSON, the model may be represented using other formats in the future.

---

# 2. Top-Level Structure

The Issue Context consists of five top-level sections.

```
issue-context.json

├── metadata

├── parentIssue

├── childIssues

├── pullRequests

└── repositoryChanges
```

---

# 3. Metadata

Purpose

Provides metadata describing the Issue Context itself.

| Field | Type | Required | Source | Description |
|--------|------|----------|--------|-------------|
| schemaVersion | String | Yes | Context API | Issue Context schema version |
| generatedAt | DateTime | Yes | Context API | Generation timestamp |
| parentIssueId | String | Yes | Linear | Parent Issue identifier |

---

# 4. Parent Issue

Purpose

Provides the approved planning information for the feature.

| Field | Type | Required | Source | Description |
|--------|------|----------|--------|-------------|
| id | String | Yes | Linear | Parent Issue identifier |
| title | String | Yes | Linear | Parent Issue title |
| description | Markdown | Yes | Linear | Parent Issue description |
| acceptanceCriteria | Markdown | Yes | Linear | Acceptance criteria |
| labels | Array | No | Linear | Labels |
| status | String | Yes | Linear | Current status |

---

# 5. Child Issues

Purpose

Provides the implementation breakdown.

Each Child Issue contains:

| Field | Type | Required | Source | Description |
|--------|------|----------|--------|-------------|
| id | String | Yes | Linear | Child Issue identifier |
| title | String | Yes | Linear | Child Issue title |
| description | Markdown | Yes | Linear | Child Issue description |
| status | String | Yes | Linear | Current status |
| labels | Array | No | Linear | Labels |

---

# 6. Pull Requests

Purpose

Provides implementation facts.

Each Pull Request contains:

| Field | Type | Required | Source | Description |
|--------|------|----------|--------|-------------|
| number | Integer | Yes | GitHub | Pull Request number |
| title | String | Yes | GitHub | Pull Request title |
| description | Markdown | Yes | GitHub | Pull Request description |
| author | String | Yes | GitHub | PR author |
| mergedAt | DateTime | Yes | GitHub | Merge timestamp |
| linkedChildIssue | String | Yes | GitHub / Linear | Associated Child Issue |

---

# 7. Repository Changes

Purpose

Describes implementation changes to the repository.

Each changed file contains:

| Field | Type | Required | Source | Description |
|--------|------|----------|--------|-------------|
| path | String | Yes | GitHub | Repository path |
| changeType | Enum | Yes | GitHub | Added, Modified, Deleted, Renamed |

---

# 8. Ownership

Every section has exactly one owner.

| Section | Owner |
|----------|-------|
| metadata | Context API |
| parentIssue | Linear |
| childIssues | Linear |
| pullRequests | GitHub |
| repositoryChanges | GitHub |

No section may have multiple owners.

---

# 9. Serialization

The current serialization format is JSON.

The logical model is independent of serialization.

Consumers should rely on field semantics rather than document formatting.

---

# 10. Example Structure

```text
issue-context.json

metadata

parentIssue

childIssues[]

pullRequests[]

repositoryChanges[]
```

---

# 11. Future Evolution

Future versions may introduce additional sections when required.

Examples include:

- Releases
- Deployments
- Test Results

Future additions must satisfy the principles defined in the Issue Context Specification.

Reasoning and AI-generated conclusions must never become part of the Issue Context Model.
