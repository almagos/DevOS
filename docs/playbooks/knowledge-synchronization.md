# Knowledge Synchronization

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Canonical Knowledge
>
> This playbook defines the workflow for synchronizing Canonical Knowledge with implemented reality.
>
> Knowledge Synchronization is responsible for ensuring that repository documentation accurately reflects completed and validated implementation.

---

# 1. Objective

The objective of Knowledge Synchronization is to synchronize Canonical Knowledge with implemented reality.

The workflow ensures that:

- Repository documentation remains accurate.
- Documentation drift is prevented.
- Canonical Knowledge remains the single source of truth.
- Documentation reflects validated implementation rather than planned work.

Knowledge Synchronization is a repository maintenance workflow.

It is not part of implementation.

---

# 2. Trigger

Knowledge Synchronization begins only after:

- The Parent Issue has been completed.
- All associated Child Issues have been completed.
- All implementation Pull Requests have been merged.
- Implementation has been validated.

Knowledge Synchronization must never begin before implementation is complete.

---

# 3. Inputs

The workflow requires the following inputs.

| Input | Source of Truth |
|---------|----------------|
| Repository | GitHub Repository |
| AGENTS.md | Repository |
| Documentation Architecture | Repository |
| Repository Structure | Repository |
| Issue Context | `.devos/issues/<parent>/issue-context.json` |

No additional lookups into external systems should be required.

---

# 4. Outputs

Knowledge Synchronization produces:

- Updated Canonical Knowledge
- New documentation when required
- Removed obsolete documentation
- Knowledge Synchronization Report

The Knowledge Synchronization Report is stored under:

```
.devos/issues/<parent>/knowledge-sync-report.md
```

---

# 5. Workflow

## Step 1

Read repository bootstrap documentation.

Read:

- AGENTS.md
- Documentation Architecture
- Repository Structure

---

## Step 2

Load the Issue Context.

The Issue Context provides the complete factual representation of the completed Parent Issue.

---

## Step 3

Understand implemented reality.

Review:

- Parent Issue
- Child Issues
- Pull Requests
- Repository Changes

Determine what has actually been implemented.

Do not reason from planned work alone.

---

## Step 4

Identify affected Canonical Knowledge.

Determine:

- Which documents require updates.
- Which documents require creation.
- Which documents have become obsolete.

Always prefer updating existing Canonical Knowledge before creating new documents.

---

## Step 5

Update Canonical Knowledge.

Update documentation to accurately represent implemented reality.

Documentation must remain:

- Accurate
- Complete
- Non-duplicated
- Consistent

---

## Step 6

Validate repository consistency.

Confirm:

- No duplicate knowledge exists.
- Every document has one canonical home.
- Cross references remain valid.
- Documentation architecture remains consistent.

---

## Step 7

Generate the Knowledge Synchronization Report.

The report should summarize:

- Documentation updated
- Documentation created
- Documentation removed
- Manual follow-up items
- Validation results

---

# 6. Decision Rules

Knowledge Synchronization follows the following decision rules.

## Rule 1

Implementation always overrides planning.

---

## Rule 2

Repository documentation reflects implemented reality.

---

## Rule 3

Every knowledge change has one canonical location.

---

## Rule 4

Prefer updating existing documentation over creating new documentation.

---

## Rule 5

Do not duplicate knowledge.

Cross-reference existing documentation instead.

---

## Rule 6

Generated operational artifacts never become Canonical Knowledge.

---

## Rule 7

When uncertainty exists, preserve repository consistency rather than creating additional documentation.

---

# 7. Validation

Knowledge Synchronization is complete when:

- All required documentation has been updated.
- Documentation accurately reflects implemented reality.
- No obsolete knowledge remains.
- Repository navigation remains consistent.
- Documentation passes repository standards.

---

# 8. Failure Handling

Knowledge Synchronization should stop if:

- Required inputs are missing.
- Issue Context is invalid.
- Repository structure cannot be determined.
- Canonical location cannot be identified.

Do not guess.

Do not invent repository structure.

Do not create undocumented knowledge.

---

# 9. Related Standards

Applicable standards include:

- Documentation Standard
- Repository Standard
- Naming Standard
- Writing Standard

---

# 10. Related Templates

Applicable templates include:

- Feature Template
- Architecture Template
- Pattern Template
- ADR Template
- Runbook Template

---

# 11. Related Documents

Repository Constitution

- AGENTS.md
- Documentation Architecture
- Repository Structure

Repository Contracts

- Issue Context Specification
- Issue Context Model
