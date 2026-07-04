# Planning

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Planning Lifecycle Stage
>
> This playbook defines how ideas are transformed into approved work ready for implementation.
>
> Planning establishes scope, priorities, and implementation boundaries before development begins.

---

# Lifecycle Position

```
Idea

↓

Planning

↓

Implementation
```

---

# 1. Objective

The objective of the Planning workflow is to transform an idea into a well-defined, approved Parent Issue with an executable implementation plan.

Planning is responsible for:

- Understanding the problem
- Defining the desired outcome
- Establishing implementation scope
- Identifying work breakdown
- Obtaining required approvals

Planning does not produce implementation.

Planning does not update Canonical Knowledge.

---

# 2. Trigger

Planning begins when:

- A new idea is proposed.
- A product improvement is requested.
- A defect requires structured implementation.
- Existing functionality requires enhancement.

---

# 3. Inputs

| Input | Source |
|--------|--------|
| Idea | Human |
| Product Vision | Repository |
| Existing Documentation | Repository |
| Existing Repository | GitHub |

---

# 4. Outputs

| Output | Destination |
|---------|-------------|
| Approved Parent Issue | Linear |
| Child Issues | Linear |
| Acceptance Criteria | Parent Issue |
| Implementation Scope | Parent Issue |

---

# 5. Workflow

## Step 1

Understand the problem.

Determine:

- Why the work is needed.
- Who benefits.
- Expected outcome.

---

## Step 2

Review existing knowledge.

Review relevant:

- Product documentation
- Engineering documentation
- Existing features
- Repository architecture

Avoid creating duplicate functionality.

---

## Step 3

Define implementation scope.

Document:

- Goals
- Scope
- Out of Scope
- Acceptance Criteria

---

## Step 4

Break work into Child Issues.

Each Child Issue should represent one independently implementable unit of work.

Every Child Issue must belong to exactly one Parent Issue.

---

## Step 5

Obtain approval.

Planning concludes only after the Parent Issue has been reviewed and approved.

---

# 6. Decision Rules

Planning follows the following rules.

## Rule 1

Every implementation begins with one Parent Issue.

---

## Rule 2

Every Child Issue belongs to exactly one Parent Issue.

---

## Rule 3

Planning defines intent, not implementation.

---

## Rule 4

Acceptance Criteria must be testable.

---

## Rule 5

Scope should minimize unnecessary implementation.

---

## Rule 6

Planning should reuse existing repository knowledge whenever possible.

---

# 7. Validation

Planning is complete when:

- The problem is clearly understood.
- Scope has been approved.
- Acceptance Criteria are complete.
- Child Issues have been created.
- The Parent Issue has been approved.

---

# 8. Failure Handling

Planning should stop when:

- Requirements are unclear.
- Scope cannot be defined.
- Acceptance Criteria cannot be written.
- Required approvals have not been obtained.

Resolve planning deficiencies before implementation begins.

---

# 9. Exit Criteria

Planning is complete when:

- One approved Parent Issue exists.
- Required Child Issues exist.
- Implementation scope has been approved.

---

# 10. Next Stage

Successful completion transfers control to the Implementation workflow.

```
Planning

↓

Implementation
```

---

# 11. Related Documents

## Repository Constitution

- AGENTS.md
- Documentation Architecture
- Repository Structure

## Related Playbooks

- Implementation
- Validation
- Knowledge Synchronization
- Release
