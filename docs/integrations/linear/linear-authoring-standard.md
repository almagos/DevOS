# Linear Authoring Standard

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Linear Integration
>
> This standard defines how DevOS planning artifacts are authored within Linear.
>
> All Parent Issues and Child Issues created in Linear must comply with this standard.

---

# 1. Purpose

This standard defines how DevOS planning artifacts are represented within Linear.

Linear is the Source of Truth for planning.

Each Parent Issue and Child Issue should follow a consistent structure to ensure predictable planning, implementation, and execution by both humans and AI agents.

---

# 2. Repository References

The structure of every Linear Issue is defined by the following repository documents.

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

## Repository Vocabulary

- `docs/glossary.md`

## Related Playbooks

- `docs/playbooks/planning.md`

## Related Standards

- `docs/standards/writing-standard.md`
- `docs/standards/naming-standard.md`

## Related Templates

- `docs/templates/linear-issue-template.md`

---

# 3. DevOS ↔ Linear Mapping

| DevOS | Linear | API Field |
|--------|--------|-----------|
| Parent Issue / Child Issue | Issue | `title` |
| Planning Artifact | Issue Description | `description` |
| Project | Project | `projectId` |
| Labels | Labels | `labelIds` |
| Priority | Priority | `priority` |
| Parent Issue | Parent Issue | `parentId` |

---

# 4. Runtime Configuration

Runtime configuration is provided externally.

Required variables include:

- `LINEAR_API_KEY`
- `TEAM_ID`
- `PROJECT_ID`
- `DEFAULT_PRIORITY`

These values must never be hardcoded.

---

# 5. Authoring Rules

All Linear Issues must follow these rules.

- Every issue represents exactly one Parent Issue or one Child Issue.
- The Issue title should contain only the issue title.
- The Issue description should follow the Linear Issue Template.
- Use GitHub-Flavored Markdown.
- Reuse existing repository knowledge whenever possible.
- Reference existing documentation rather than duplicating knowledge.
- Use repository terminology defined in the Glossary.
- Planning should define intent rather than implementation.

---

# 6. Linear Field Mapping

| Repository Artifact | Linear API |
|---------------------|------------|
| Issue Title | `title` |
| Issue Description | `description` |
| Labels | `labelIds` |
| Parent Issue | `parentId` |
| Priority | `priority` |

---

# 7. Authoring Workflow

1. Review the Planning Playbook.
2. Review relevant repository documentation.
3. Review applicable repository standards.
4. Use the Linear Issue Template.
5. Select the appropriate labels.
6. Populate the Parent Issue or Child Issue.
7. Validate the completed issue.
8. Submit the GraphQL payload using Bruno.

---

# 8. Canonical GraphQL Payload

```json
{
  "input": {
    "teamId": "{{TEAM_ID}}",
    "projectId": "{{PROJECT_ID}}",
    "priority": {{DEFAULT_PRIORITY}},
    "labelIds": [
      "<LABEL_UUID>",
      "<LABEL_UUID>",
      "<LABEL_UUID>"
    ],
    "title": "<Issue Title>",
    "description": "<Issue Description>"
  }
}
```

---

# 9. Label Selection Rules

- Select exactly one Domain label.
- Select exactly one Area label.
- Select exactly one Work label.
- Select exactly one Lifecycle label.
- Executor labels are optional.
- Do not assign label category labels (`Domain`, `Area`, `Work`, `Lifecycle`, `Executor`).

---

# 10. Label UUID Registry

## Domain

| Label | UUID |
|--------|------|
| Feature | 88a090c1-f41a-46ac-948d-601b1387a880 |
| Bug | 334118eb-8224-4ba4-b071-7f5d4bf4f721 |
| Requirement | e87479f1-b460-42b2-80e8-19e3167084b1 |
| Pattern | fe11c318-6e90-42b7-b2ca-75290c58ac8a |
| Decision | 8c1dc12b-b7a8-4559-be9a-35ef514b9396 |
| Standard | a6a90837-5f14-44b0-a07b-af2958f37284 |
| Architecture | 88ac4f5e-7322-4c95-90dd-dcccdef3f4d6 |
| Research | 855b4ce7-150c-4b2e-b39e-8219fd87caa9 |
| Runbook | d3496ad3-261a-44e8-beec-7dc20d05fc97 |
| Chore | 7f04aca8-e4fc-4b0f-8884-bde7a8e70a96 |

## Area

| Label | UUID |
|--------|------|
| UI | 999a3775-33de-42d4-bbb3-d3d8e41c7c3c |
| Auth | 5eeff93f-ccc6-4b39-a8d1-faf91e04ba4b |
| API | dd53648d-e2c5-43d4-937a-ce9b7da85fe0 |
| Database | 2f24a680-6f85-47a3-b8b1-155c0f97e97e |
| Workflow | 0f178640-8ed9-4616-8df6-7f61e6c3aa15 |
| Deployment | fe5bbb63-81bf-4192-a95c-541e7a943b73 |
| Security | f41c1c86-893f-4a2f-b72b-7a3b7be13277 |
| Observability | 40082da2-26e4-41a8-97e7-598f6aeafc84 |
| Automation | 1449ad94-0450-4b4f-a764-e6e37849303a |
| DevOS | 39f95d5a-28f1-475c-bde7-3d4f6454a409 |
| Docs | b621ff6e-3f56-4405-a1ac-b96763cc1510 |
| GitHub | 8e328469-23c4-4a95-8f84-0e92540f4008 |
| Linear | 7e22bdab-0f12-4277-8829-74afb6b8884e |
| Supabase | 2ce2a6da-fc4e-4d25-9172-fa3f5cc6bcea |

## Work

| Label | UUID |
|--------|------|
| Specification | da48cdc2-a5ff-4e09-9878-4394555d9cf4 |
| Implementation | 32b0e74b-d0e9-4e8c-9945-91d550370d80 |
| Documentation | 373bf0be-2e7a-4dfb-8952-61a3fbcc27b0 |
| Refactor | 17463a9c-52b9-43f2-a55d-63010e739f7d |
| Testing | d8e48674-8bc9-485f-947e-d4f294d24ba7 |
| Migration | 8dcfc578-df5d-4170-99bd-e8c36c5fa8d6 |
| Maintenance | 1e21b6da-e841-4815-9ba5-e80b99308885 |

## Lifecycle

| Label | UUID |
|--------|------|
| Planning | e353dfe3-fa82-4330-b26e-9ed87a949583 |
| Approved | 773ef48f-3a11-4518-b1f2-331444a96433 |
| Ready for Engineering | 2e20b84c-f835-46b5-b99c-7a0f9811b1cc |
| Blocked | cdfca58f-06aa-4330-ae9c-6333307f640f |
| Deferred | e6ffc3ee-7c74-4d67-9299-aa47ce861781 |

## Executor

| Label | UUID |
|--------|------|
| Human | 97120c74-bf8e-41f4-90f8-1717df614202 |
| ChatGPT | 6f95ad83-de00-4fa0-ad9d-10d7488a39c9 |
| Claude | a9e3d3f2-7107-4132-bcb4-7b33a5a7cf50 |
| Codex | c9a9f256-8603-4019-bea0-816f24ec6f66 |
| System | 5d78f3de-f9eb-4316-86eb-07a24463455a |

---

# 11. Authoring Checklist

- [ ] Planning Playbook reviewed.
- [ ] Repository documentation reviewed.
- [ ] Applicable standards reviewed.
- [ ] Linear Issue Template followed.
- [ ] Issue title finalized.
- [ ] Issue description completed.
- [ ] Domain label selected.
- [ ] Area label selected.
- [ ] Work label selected.
- [ ] Lifecycle label selected.
- [ ] UUIDs copied from the registry.
- [ ] Bruno variables used.
- [ ] Markdown validated.

---

# 12. Related Documents

## Repository Constitution

- `AGENTS.md`
- `docs/engineering/repository/documentation-architecture.md`
- `docs/engineering/repository/repository-structure.md`

## Repository Vocabulary

- `docs/glossary.md`

## Related Playbooks

- `docs/playbooks/planning.md`

## Related Templates

- `docs/templates/linear-issue-template.md`
