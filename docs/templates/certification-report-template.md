# Certification Report Template

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Repository Certification
>
> This template defines the canonical structure for all DevOS certification reports.
>
> Every certification process should produce a report using this template.

---

# Purpose

Certification reports document the outcome of a repository evaluation.

They provide a structured assessment of repository quality, identify findings, and record recommendations.

Certification reports evaluate repository state.

They do not prescribe implementation.

---

# Certification Information

| Field | Value |
|--------|-------|
| Certification | |
| Repository | |
| Repository Version | |
| Date | |
| Auditor | |
| DevOS Version | |

---

# Executive Summary

Provide a concise summary of the certification.

Include:

- overall assessment
- major strengths
- major risks
- certification outcome

---

# Scope

Describe what was evaluated.

Examples:

- Repository Architecture
- Documentation
- Playbooks
- Standards
- Templates
- Integrations
- Generated Operational State

---

# Methodology

Describe how the certification was performed.

Examples:

- Recursive documentation traversal
- Link validation
- Terminology validation
- Workflow reconstruction
- Source of Truth verification
- AI onboarding simulation

---

# Findings

## Strengths

List notable strengths identified during certification.

---

## Issues

List every issue discovered.

For each issue include:

| Severity | Area | Description | Recommendation |
|----------|------|-------------|----------------|

Severity should be one of:

- Critical
- Important
- Optional

---

# Metrics

Record measurable certification metrics.

Examples:

| Metric | Value |
|--------|-------|
| Documents Reviewed | |
| README Files Reviewed | |
| Links Validated | |
| Broken Links Found | |
| Broken Links Fixed | |
| Terminology Issues | |
| Architecture Issues | |
| Workflow Issues | |

Only include metrics applicable to the certification.

---

# Recommendations

Group recommendations by priority.

## Critical

Items that should be addressed before certification.

---

## Important

Items that should be addressed in the next improvement cycle.

---

## Optional

Suggested improvements that are not required for certification.

---

# Certification Result

Choose one outcome.

- ✅ Certified
- ⚠️ Certified with Recommendations
- ❌ Not Certified

Provide the reasoning.

---

# Readiness Assessment

Score each category from 1–10.

| Category | Score | Notes |
|----------|------:|-------|
| Documentation | |
| Architecture | |
| Consistency | |
| Navigation | |
| AI Readiness | |
| Human Readability | |
| Automation Readiness | |
| Maintainability | |

Add or remove categories depending on the certification.

---

# Next Steps

Describe the recommended follow-up actions.

Examples:

- Fix Critical findings
- Update repository documentation
- Re-run certification
- Release repository
- Schedule compliance audit

---

# Related Documents

## Related Playbooks

List applicable playbooks.

---

## Related Standards

List applicable standards.

---

## Related Templates

List applicable templates.

---

# Certification History

| Date | Certification | Result | Auditor |
|------|---------------|--------|----------|

Append a new entry for each certification rather than modifying previous results.
