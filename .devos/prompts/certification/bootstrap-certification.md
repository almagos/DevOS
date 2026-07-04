# Bootstrap Certification Prompt

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
> **Related Template:** `docs/templates/certification-report-template.md`

---

# Purpose

This prompt executes the DevOS Bootstrap Certification Playbook.

Its purpose is to evaluate whether a repository is capable of onboarding autonomous AI agents and human contributors using only its documented knowledge.

The prompt performs certification only.

It must not modify the repository.

---

# Prerequisites

Before executing this prompt ensure that:

- The repository contains `AGENTS.md`.
- The Bootstrap Certification Playbook exists.
- The Certification Report Template exists.
- All documentation changes have been committed.

Bootstrap Certification evaluates a repository at a point in time.

Material documentation changes invalidate previous certification results.

---

# Inputs

Repository root.

Required documents:

- `AGENTS.md`
- `docs/playbooks/bootstrap-certification.md`
- `docs/templates/certification-report-template.md`

---

# Prompt

Execute the DevOS Bootstrap Certification Playbook.

Playbook:

`docs/playbooks/bootstrap-certification.md`

Certification Report Template:

`docs/templates/certification-report-template.md`

## Objective

Perform a complete Bootstrap Certification of the repository using the documented DevOS certification process.

Execute the playbook exactly as written.

Generate the certification report using the canonical Certification Report Template.

---

## Scope

Evaluate the repository exactly as it exists.

Do not modify repository files.

Do not implement fixes.

Do not propose architectural redesign unless a genuine architectural issue exists.

This is a certification exercise only.

---

## Validation Requirements

Execute every validation defined by the Bootstrap Certification Playbook, including:

- Repository Bootstrap
- Documentation Navigation
- Documentation Architecture
- Repository Consistency
- Terminology
- Workflow Reconstruction
- Integration Boundaries
- Generated Operational State
- AI Onboarding
- Human Onboarding
- Source of Truth Verification

Perform a complete recursive traversal beginning with `AGENTS.md`.

---

## Bootstrap Trace

Include a complete Bootstrap Trace documenting:

- every document visited
- why it was visited
- which document referenced it
- what knowledge it contributed
- what additional references it introduced

The trace should demonstrate exactly how a first-time autonomous AI agent bootstraps itself using DevOS.

---

## Certification Report

Generate the report using:

`docs/templates/certification-report-template.md`

Populate every applicable section.

Include:

- Executive Summary
- Scope
- Methodology
- Findings
- Metrics
- Recommendations
- Readiness Assessment
- Next Steps
- Certification Result

---

## Recommendations

Classify findings as:

- Critical
- Important
- Optional

Recommend only changes that materially improve DevOS.

Avoid stylistic recommendations.

Avoid speculative future enhancements.

---

## Final Assessment

Determine whether the repository is ready for public release as the canonical DevOS repository or GitHub Template Repository.

Conclude with one of:

- ✅ DevOS Certified
- ⚠️ DevOS Certified with Recommendations
- ❌ DevOS Not Yet Ready

Provide justification for the outcome.

---

## Release Readiness

If the repository is certified, include a final Release Readiness Assessment confirming whether it is ready to:

- be tagged with a release
- be published
- be used as the canonical implementation

If certification is withheld, clearly identify the blocking issues.

---

## Constraints

- Do not modify repository files.
- Do not implement fixes.
- Do not create new documentation.
- Evaluate only the repository's current state.
- Treat the certification as a point-in-time assessment.

---

# Deliverables

Produce a single Certification Report conforming to the Certification Report Template.

No repository modifications should be made.

---

# Success Criteria

The prompt succeeds when:

- The Bootstrap Certification Playbook has been fully executed.
- Every required validation has been completed.
- A Certification Report has been generated.
- The repository receives a clear certification outcome.
- All findings are classified by severity.

---

# Related Documentation

## Playbooks

- `docs/playbooks/bootstrap-certification.md`

## Templates

- `docs/templates/certification-report-template.md`

## Standards

- `docs/standards/documentation-standard.md`

## Repository Constitution

- `AGENTS.md`
