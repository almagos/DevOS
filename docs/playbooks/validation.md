# Validation

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Validation Lifecycle Stage
>
> This playbook defines how completed implementation is validated before Knowledge Synchronization begins.
>
> Validation ensures that implemented reality satisfies approved planning and repository quality standards.

---

# Lifecycle Position

```
Implementation

↓

Validation

↓

Knowledge Synchronization
```

---

# 1. Objective

The objective of the Validation workflow is to confirm that implementation is complete, correct, and ready to become Canonical Knowledge.

Validation is responsible for:

- Verifying implementation completeness
- Verifying repository quality
- Confirming acceptance criteria
- Identifying implementation defects
- Determining readiness for Knowledge Synchronization

Validation does not update repository documentation.

---

# 2. Trigger

Validation begins when:

- All Child Issues have been implemented.
- All Pull Requests have been merged.
- Implementation is complete.

---

# 3. Inputs

| Input | Source of Truth |
|---------|----------------|
| Parent Issue | Linear |
| Child Issues | Linear |
| Repository | GitHub |
| Issue Context | `.devos/issues/<parent>/issue-context.json` |
| Merged Pull Requests | GitHub |

---

# 4. Outputs

| Output | Destination |
|---------|-------------|
| Validation Result | Parent Issue |
| Validation Findings | Parent Issue |
| Approval Decision | Parent Issue |

---

# 5. Workflow

## Step 1

Review the completed Parent Issue.

Verify that all associated Child Issues have been completed.

---

## Step 2

Review implementation.

Verify:

- All Pull Requests have been merged.
- Repository state is consistent.
- Implementation scope matches approved planning.

---

## Step 3

Verify acceptance criteria.

Confirm that every acceptance criterion defined in the Parent Issue has been satisfied.

---

## Step 4

Review repository quality.

Verify:

- Repository standards have been followed.
- No incomplete implementation remains.
- No unintended changes exist.

---

## Step 5

Record validation outcome.

Validation concludes with one of the following outcomes:

- Approved
- Changes Required

---

# 6. Decision Rules

Validation follows the following rules.

## Rule 1

Validation verifies implementation.

It does not modify implementation.

---

## Rule 2

Only completed implementation may be validated.

---

## Rule 3

Every acceptance criterion must be evaluated.

---

## Rule 4

Repository quality is evaluated alongside functional correctness.

---

## Rule 5

Validation findings must be resolved before proceeding.

---

# 7. Validation

Validation is considered complete when:

- All acceptance criteria have been evaluated.
- Repository quality has been confirmed.
- Validation outcome has been recorded.

---

# 8. Failure Handling

Validation should stop when:

- Required implementation is incomplete.
- Acceptance criteria cannot be evaluated.
- Repository inconsistencies are detected.
- Required information is missing.

Return control to the Implementation workflow until deficiencies have been resolved.

---

# 9. Exit Criteria

Validation is complete when:

- Implementation has been approved.
- Repository quality has been confirmed.
- Acceptance criteria have been satisfied.

---

# 10. Next Stage

Successful completion transfers control to the Knowledge Synchronization workflow.

```
Validation

↓

Knowledge Synchronization
```

---

# 11. Related Documents

## Repository Constitution

- AGENTS.md
- Documentation Architecture
- Repository Structure

## Context Layer

- Issue Context Specification
- Issue Context Model

## Related Playbooks

- Implementation
- Knowledge Synchronization
- Release
