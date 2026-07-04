# Release

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Release Lifecycle Stage
>
> This playbook defines how validated work becomes an official repository release.
>
> Release marks the completion of the development lifecycle for a Parent Issue.

---

# Lifecycle Position

```
Knowledge Synchronization

↓

Release

↓

Completed
```

---

# 1. Objective

The objective of the Release workflow is to finalize completed work after implementation, validation, and Knowledge Synchronization have been successfully completed.

Release is responsible for:

- Confirming repository readiness
- Confirming Canonical Knowledge is synchronized
- Completing the Parent Issue lifecycle
- Recording release completion

Release does not modify implementation or documentation.

---

# 2. Trigger

Release begins when:

- Validation has been completed.
- Knowledge Synchronization has been completed.
- Canonical Knowledge accurately reflects implemented reality.

---

# 3. Inputs

| Input | Source of Truth |
|---------|----------------|
| Repository | GitHub |
| Parent Issue | Linear |
| Knowledge Synchronization Report | `.devos/issues/<parent>/knowledge-sync-report.md` |

---

# 4. Outputs

| Output | Destination |
|---------|-------------|
| Released Parent Issue | Linear |
| Release Tag (Optional) | GitHub |
| Deployment (Optional) | Deployment Platform |

---

# 5. Workflow

## Step 1

Confirm Validation has been successfully completed.

---

## Step 2

Confirm Knowledge Synchronization has completed successfully.

Verify:

- Canonical Knowledge has been updated.
- Repository documentation is consistent.
- Knowledge Synchronization Report exists.

---

## Step 3

Confirm repository readiness.

Verify:

- Repository is in a releasable state.
- No blocking issues remain.
- Repository standards continue to be satisfied.

---

## Step 4

Complete the Parent Issue lifecycle.

Mark the Parent Issue as Released.

---

## Step 5

Perform release activities.

Examples include:

- Creating a release tag.
- Deploying the application.
- Publishing release notes.

These activities depend on the project and deployment strategy.

---

# 6. Decision Rules

Release follows the following rules.

## Rule 1

Release only validated implementation.

---

## Rule 2

Release only synchronized knowledge.

---

## Rule 3

Canonical Knowledge must accurately represent implemented reality before release.

---

## Rule 4

Release activities are project-specific.

The Release workflow defines when release occurs, not how deployment is performed.

---

# 7. Validation

Release is complete when:

- The Parent Issue has been released.
- Required release activities have been completed.
- Repository remains consistent.

---

# 8. Failure Handling

Release should stop when:

- Validation has not completed.
- Knowledge Synchronization has not completed.
- Repository readiness cannot be confirmed.
- Blocking issues remain unresolved.

Resolve failures before continuing.

---

# 9. Exit Criteria

Release is complete when:

- The Parent Issue lifecycle has ended.
- Required release activities have been completed.

---

# 10. Next Stage

```
Completed
```

The Parent Issue lifecycle ends.

Future work begins through a new Planning workflow.

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

- Validation
- Knowledge Synchronization
- Planning
