# DAS-02 — WHAT

| Metadata | Value |
| --- | --- |
| **Title** | DAS-02 — WHAT |
| **Document ID** | DAS-02 |
| **Version** | 1.0.0 |
| **Status** | Approved |
| **Parent** | AF-001 — DevOS Foundation Architecture |
| **Last Updated** | 2026-07-01 |

---

## Purpose

The WHAT dimension defines the static structure of DevOS.

It establishes the canonical domain model, the entities that compose the Development Operating System, and the relationships between those entities.

It answers one question:

> What exists within DevOS?

---

## Domain Model

```text
Organization
│
└── Project
      │
      ├── Vision
      ├── Standard
      ├── Repository
      ├── Release
      │
      └── Issue
            │
            ├── Sub-Issue
            │
            ├── Pull Request
            │      │
            │      ├── Branch
            │      └── Commit
            │
            ├── Artifact
            │      │
            │      ├── Documentation
            │      ├── Source Code
            │      ├── Tests
            │      ├── Database Changes
            │      └── Assets
            │
            └── Decision
```

---

## Entity Definitions

### Organization

Owns one or more Projects.

---

### Project

Represents a software product or initiative.

Contains work, repositories, releases and standards.

---

### Repository

The canonical implementation and knowledge repository of a project.

---

### Vision

Defines the long-term direction of a project.

---

### Standard

Defines reusable operating rules.

Standards are version-controlled artifacts.

---

### Issue

A planned unit of work.

Every meaningful change begins as an Issue.

---

### Sub-Issue

A decomposition of an Issue into executable work.

---

### Pull Request

Represents the implementation of an Issue.

Every Issue produces one primary Pull Request.

---

### Branch

An isolated implementation workspace.

Branch names follow the work management platform convention.

---

### Commit

A version-controlled checkpoint within a Branch.

---

### Artifact

A persistent output produced by an Issue.

Artifacts are version controlled.

---

### Documentation

Architecture, standards and implementation knowledge.

Documentation is a first-class Artifact.

---

### Source Code

Executable implementation artifacts.

---

### Tests

Validation artifacts.

---

### Database Changes

Schema and data evolution artifacts.

---

### Assets

Images, icons, diagrams and other project resources.

---

### Decision

Recorded architectural or product decisions.

---

### Release

A deliverable version of a Project.

---

## Relationships

| Source | Relationship | Target |
| --- | --- | --- |
| Organization | owns | Project |
| Project | contains | Issue |
| Issue | may contain | Sub-Issue |
| Issue | produces | Pull Request |
| Pull Request | implemented on | Branch |
| Branch | contains | Commit |
| Pull Request | modifies | Artifact |
| Artifact | stored in | Repository |
| Project | governed by | Standard |
| Project | guided by | Vision |
| Project | produces | Release |

---

## Core Rules

- Every Project has one canonical Repository.
- Every meaningful change begins with an Issue.
- Every Issue produces one primary Pull Request.
- Every Pull Request creates or modifies one or more Artifacts.
- Documentation is a first-class Artifact.
- Standards are first-class Artifacts.
- Documentation evolves together with implementation.

---

## Canonical Terminology

DevOS adopts platform terminology wherever practical.

Canonical terms are:

- Organization
- Project
- Repository
- Issue
- Sub-Issue
- Pull Request
- Branch
- Commit
- Artifact
- Release

No additional abstraction layer is introduced in DevOS v1.

---

## Success Criteria

- Every DevOS concept maps to a defined entity.
- Every entity has a defined responsibility.
- Relationships are explicit.
- Future standards derive from this domain model.
