# DevOS Prompt Library

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** AI-Assisted Repository Operations
>
> This directory contains reusable prompts for executing DevOS workflows using AI assistants.

---

# Purpose

The Prompt Library provides standardized prompts that operationalize DevOS.

Each prompt is designed to execute an established repository workflow defined by the DevOS documentation.

Prompts are convenience artifacts that help AI assistants execute repository processes consistently.

They are **not** the canonical definition of repository behavior.

---

# Relationship to DevOS

DevOS separates repository knowledge from AI execution.

```
Playbooks
│
├── Define repeatable workflows.
│
▼
Templates
│
├── Define the expected output.
│
▼
Prompts
│
└── Instruct AI assistants to execute the workflow.
```

The repository documentation always remains the Source of Truth.

Prompts simply operationalize that knowledge.

---

# Repository Structure

```
.devos/prompts/

├── README.md
│
├── certification/
│   Repository certification prompts.
│
├── planning/
│   Planning workflow prompts.
│
├── implementation/
│   Implementation workflow prompts.
│
├── validation/
│   Validation workflow prompts.
│
├── knowledge/
│   Knowledge Synchronization prompts.
│
└── release/
    Release workflow prompts.
```

---

# Prompt Principles

Every prompt should:

- Execute an existing DevOS workflow.
- Reference canonical repository documentation.
- Avoid duplicating repository knowledge.
- Produce deterministic outputs.
- Be reusable across repositories using DevOS.
- Be compatible with multiple AI assistants whenever practical.

---

# Prompt Structure

Every prompt should follow a consistent structure.

1. Purpose
2. Prerequisites
3. Inputs
4. Instructions
5. Constraints
6. Deliverables
7. Success Criteria
8. Related Documentation

This keeps prompts consistent across the repository.

---

# Supported AI Assistants

The prompts are intended to be portable across AI assistants.

Examples include:

- ChatGPT
- Claude
- Codex
- Antigravity

Prompts should avoid provider-specific behavior whenever possible.

---

# Source of Truth

Prompt files are **not** the authoritative definition of DevOS workflows.

The Source of Truth remains:

- `docs/playbooks/`
- `docs/standards/`
- `docs/templates/`
- `AGENTS.md`

When a prompt conflicts with repository documentation, the repository documentation always takes precedence.

---

# Maintenance

Whenever a Playbook, Standard or Template changes:

1. Update the canonical documentation.
2. Review affected prompts.
3. Update prompts if required.
4. Re-run applicable certification workflows.

Prompts should always reflect the current repository architecture.

---

# Related Documents

## Repository Constitution

- `AGENTS.md`

---

## Playbooks

- `docs/playbooks/`

---

## Standards

- `docs/standards/`

---

## Templates

- `docs/templates/`

---

## Generated Operational State

- `.devos/`
