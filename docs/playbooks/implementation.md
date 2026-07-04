# Implementation

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Implementation Lifecycle Stage
>
> This playbook defines how approved work is implemented within the repository.
>
> Implementation transforms approved planning into validated source code while preserving repository integrity and preparing the required context for Knowledge Synchronization.

---

# Lifecycle Position

```
Planning

↓

Implementation

↓

Validation
```

---

# 1. Objective

The objective of the Implementation workflow is to transform approved Parent and Child Issues into validated implementation.

Implementation is responsible for:

- Producing working software
- Maintaining repository quality
- Preserving implementation traceability
- Recording implementation facts
- Preparing the Parent Issue for Knowledge Synchronization

Implementation is not responsible for updating Canonical Knowledge.

Documentation updates occur during the Knowledge Synchronization workflow.

---

# 2. Trigger

Implementation begins when:

- A Parent Issue has been approved.
- A Child Issue has been approved for implementation.

Implementation should only begin after planning is complete.

---

# 3. Inputs

| Input | Source of Truth |
|---------|----------------|
| Parent Issue | Linear |
| Child Issue | Linear |
| Repository | GitHub |
| AGENTS.md | Repository |
| Repository Constitution | Repository |

---

# 4. Outputs

| Output | Destination |
|---------|-------------|
| Source Code | GitHub |
| Pull Request | GitHub |
| Updated Issue Context | `.devos/issues/<parent>/issue-context.json` |
| Completed Child Issue | Linear |

---

# 5. Workflow

## Step 1

Select the approved Child Issue.

Review:

- Parent Issue
- Child Issue
- Repository documentation

Ensure implementation intent is fully understood before writing code.

---

## Step 2

Create a dedicated implementation branch.

One Child Issue should be implemented on one branch.

---

## Step 3

Implement the approved functionality.

Implementation should:

- Follow repository standards.
- Follow established patterns.
- Preserve repository consistency.
- Avoid unrelated changes.

---

## Step 4

Perform self-validation.

Verify:

- Code compiles.
- Tests pass.
- Acceptance criteria have been satisfied.

Resolve implementation issues before creating a Pull Request.

---

## Step 5

Create a Pull Request.

The Pull Request should clearly describe:

- What was implemented.
- Why it was implemented.
- Any implementation considerations.

---

## Step 6

Complete review and merge.

Address review feedback.

Merge only after approval.

---

## Step 7

Update the Parent Issue Context.

After every merged Pull Request:

Update:

```
.devos/issues/<parent>/issue-context.json
```

Append implementation facts only.

Do not generate summaries or conclusions.

---

## Step 8

Complete the Child Issue.

Mark the Child Issue as complete.

Repeat the workflow for the next approved Child Issue.

Continue until every Child Issue belonging to the Parent Issue has been completed.

---

# 6. Decision Rules

Implementation follows the following rules.

## Rule 1

One Child Issue is implemented per branch.

---

## Rule 2

One Pull Request is created per Child Issue.

---

## Rule 3

Every Pull Request must reference its associated Child Issue.

---

## Rule 4

Every Child Issue belongs to exactly one Parent Issue.

---

## Rule 5

Every merged Pull Request updates the Parent Issue Context.

---

## Rule 6

Implementation should modify only the approved scope.

---

## Rule 7

Canonical Knowledge must not be updated during implementation.

---

# 7. Validation

Implementation is considered complete when:

- All implementation tasks are complete.
- The Pull Request has been merged.
- The Child Issue has been completed.
- The Parent Issue Context has been updated.

---

# 8. Failure Handling

Implementation should stop when:

- Repository standards cannot be satisfied.
- Required inputs are missing.
- Acceptance criteria are unclear.
- Merge conflicts remain unresolved.
- Issue Context cannot be updated.

Resolve failures before continuing.

---

# 9. Exit Criteria

Implementation is complete when:

- Every Child Issue belonging to the Parent Issue has been implemented.
- Every Pull Request has been merged.
- The Parent Issue Context contains implementation facts for every merged Pull Request.

---

# 10. Next Stage

Successful completion transfers control to the Validation workflow.

```
Implementation

↓

Validation
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

- Planning
- Validation
- Knowledge Synchronization
