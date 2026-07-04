# DevOS Compliance Audit Prompt

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
> **Related Standards:** `docs/standards/documentation-standard.md`, `docs/standards/repository-standard.md`

---

# Purpose

This prompt evaluates whether a repository continues to comply with the DevOS operating model.

Unlike Bootstrap Certification, which determines whether a repository can successfully onboard contributors, the Compliance Audit determines whether a repository has remained aligned with DevOS as it evolves.

The audit evaluates repository conformance only.

It does not modify repository files.

---

# Prerequisites

Before executing this prompt ensure that:

- Repository documentation has been synchronized.
- Repository structure reflects the implemented system.
- Outstanding implementation work has been committed.

---

# Inputs

Repository root.

Repository documentation.

Repository structure.

Generated Operational State.

---

# Prompt

Execute a complete DevOS Compliance Audit.

## Objective

Determine whether the repository continues to comply with the DevOS operating model.

Evaluate the repository against its documented:

- Constitution
- Documentation Architecture
- Repository Structure
- Playbooks
- Standards
- Templates
- Integrations

The audit should identify repository drift.

---

## Compliance Validation

Verify:

- Repository Constitution compliance
- Documentation Architecture compliance
- Repository Structure compliance
- Playbook compliance
- Standards compliance
- Template usage
- Integration documentation
- Source of Truth separation
- Generated Operational State boundaries
- Repository navigation

---

## Repository Drift

Identify deviations including:

- Undocumented repository structure
- Duplicate knowledge
- Missing documentation
- Outdated documentation
- Documentation inconsistent with implementation
- Broken repository navigation
- Untracked architectural changes
- Violations of repository standards

---

## Workflow Compliance

Determine whether repository workflows remain consistent with DevOS.

Evaluate:

- Planning
- Implementation
- Validation
- Knowledge Synchronization
- Release

Verify that documentation accurately reflects current workflows.

---

## Source of Truth Validation

Verify that ownership remains clear.

Examples include:

- Planning → Project Management System
- Implementation → Version Control
- Canonical Knowledge → docs/
- Generated Operational State → .devos/

Identify any ambiguity.

---

## Repository Consistency

Verify:

- Terminology consistency
- Naming consistency
- Directory consistency
- Cross-reference consistency
- Documentation completeness

---

## Report

Produce a Compliance Audit Report containing:

- Executive Summary
- Compliance Findings
- Repository Drift
- Standards Violations
- Workflow Deviations
- Recommendations
- Compliance Status

---

## Compliance Result

Choose one outcome:

- ✅ Fully Compliant
- ⚠️ Compliant with Recommendations
- ❌ Non-Compliant

Provide justification.

---

## Constraints

Do not modify repository files.

Do not implement fixes.

Evaluate only the current repository state.

---

# Deliverables

Produce a complete Compliance Audit Report.

No repository modifications should be made.

---

# Success Criteria

The audit succeeds when:

- Repository structure complies with DevOS.
- Documentation remains synchronized.
- Repository workflows remain consistent.
- Sources of Truth remain unambiguous.
- No architectural drift is detected.

---

# Related Documentation

## Repository Constitution

- `AGENTS.md`

## Playbooks

- `docs/playbooks/bootstrap-certification.md`

## Standards

- `docs/standards/documentation-standard.md`
- `docs/standards/repository-standard.md`

## Templates

- `docs/templates/certification-report-template.md`
