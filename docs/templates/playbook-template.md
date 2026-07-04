# <Playbook Title>

> **Status:** Draft | Stable | Deprecated
>
> **Version:** 1.0
>
> **Owner:** <Owner>
>
> **Applies To:** <Lifecycle Stage>
>
> This playbook defines the workflow for <workflow purpose>.

---

# Lifecycle Position

```
<Previous Stage>

↓

<Current Stage>

↓

<Next Stage>
```

---

# 1. Objective

Describe the purpose of this lifecycle stage.

Explain:

- Why this workflow exists.
- What responsibility it owns.
- What responsibilities it explicitly does not own.

---

# 2. Trigger

Describe the event that starts this workflow.

A playbook should have one primary trigger.

---

# 3. Inputs

| Input | Source of Truth |
|--------|-----------------|
| | |

---

# 4. Outputs

| Output | Destination |
|---------|-------------|
| | |

---

# 5. Workflow

## Step 1

Describe the first workflow step.

---

## Step 2

Describe the second workflow step.

---

## Step 3

Continue until the workflow is complete.

---

# 6. Decision Rules

List the rules governing this workflow.

## Rule 1

Description.

---

## Rule 2

Description.

---

Additional rules should be added only when they define stable repository behavior.

---

# 7. Validation

Describe how successful completion of the workflow is determined.

Validation should use objective criteria whenever possible.

---

# 8. Failure Handling

Describe when the workflow should stop.

Explain how failures should be handled.

Avoid workflow-specific implementation details.

---

# 9. Exit Criteria

Describe the conditions that must be satisfied before the workflow is considered complete.

---

# 10. Next Stage

Describe the lifecycle stage that begins after successful completion.

```
<Current Stage>

↓

<Next Stage>
```

---

# 11. Related Documents

## Repository Constitution

- AGENTS.md
- Documentation Architecture
- Repository Structure

## Related Playbooks

List related lifecycle playbooks.

## Related Standards

List applicable standards.

## Related Templates

List templates used by this workflow where applicable.
