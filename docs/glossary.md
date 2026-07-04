# Glossary

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Entire Repository
>
> This glossary defines the canonical terminology used throughout the repository.
>
> Every defined term has exactly one authoritative meaning.
>
> Repository documentation should use these terms consistently.

---

# A

## Acceptance Criteria

The measurable conditions that must be satisfied for a Parent Issue to be considered successfully implemented and validated.

---

# C

## Canonical Knowledge

The authoritative representation of implemented knowledge stored within the repository.

Canonical Knowledge is maintained under `docs/`.

---

## Child Issue

An independently implementable unit of work belonging to exactly one Parent Issue.

Each Child Issue should result in one Pull Request.

---

# D

## Definition of Done

The conditions required for a lifecycle stage to be considered complete.

Each playbook defines its own exit criteria.

---

# G

## Generated Operational State

Machine-generated operational artifacts stored under `.devos/`.

Generated Operational State is reproducible and is never a source of truth.

---

# I

## Idea

A proposed improvement, feature, enhancement, or defect before formal planning begins.

Ideas enter the Planning workflow.

---

## Implementation

The lifecycle stage responsible for transforming approved planning into working software.

---

## Issue Context

A machine-generated, self-contained factual representation of a completed Parent Issue.

The Issue Context provides the inputs required for Knowledge Synchronization.

---

# K

## Knowledge Synchronization

The workflow responsible for updating Canonical Knowledge to reflect implemented reality.

---

# P

## Parent Issue

The primary planning artifact representing a feature, initiative, or body of work.

A Parent Issue owns one or more Child Issues.

---

## Playbook

A document describing a repeatable workflow within the DevOS lifecycle.

Playbooks define how work moves through the system.

---

# R

## Repository Constitution

The foundational documents that govern repository organization and operation.

The Repository Constitution consists of:

- AGENTS.md
- Documentation Architecture
- Repository Structure

---

## Runbook

A document describing a repeatable operational procedure.

Runbooks explain how to perform operational tasks.

---

# S

## Source of Truth

The authoritative owner of a particular category of information.

Every category of information has exactly one Source of Truth.

---

## Standard

A document defining rules and constraints that govern repository behavior.

Standards define what must always remain true.

---

# T

## Template

A reusable starting point for creating recurring repository documents.

Templates improve consistency.

---

# V

## Validation

The lifecycle stage responsible for confirming implementation satisfies approved planning and repository quality standards.

---

# W

## Workflow

A defined sequence of activities that transforms work from one lifecycle stage to another.

---

# Maintenance

The glossary should evolve conservatively.

New terms should be added only when they represent stable repository concepts.

Existing definitions should be revised only when repository architecture changes.
