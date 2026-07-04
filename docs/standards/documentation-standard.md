# Documentation Standard

> **Status:** Stable
>
> **Version:** 1.0
>
> **Owner:** DevOS
>
> **Applies To:** Repository Documentation
>
> This standard defines the rules governing repository documentation.
>
> All repository documentation must comply with this standard.

---

# 1. Purpose

The purpose of this standard is to ensure repository documentation remains:

- Accurate
- Consistent
- Discoverable
- Maintainable
- AI-friendly
- Free from duplication

Documentation is treated as a first-class engineering artifact.

---

# 2. Scope

This standard applies to all documentation stored under:

```
docs/
```

It also applies to:

```
AGENTS.md
```

It does not apply to:

```
.devos/
```

Generated operational artifacts are governed by their respective workflows.

---

# 3. Documentation Principles

All documentation follows these principles.

## Principle 1

Repository documentation represents implemented reality.

---

## Principle 2

Every piece of knowledge has exactly one canonical location.

---

## Principle 3

Documentation must not duplicate existing knowledge.

Cross references should be used instead.

---

## Principle 4

Documentation should be updated through the Knowledge Synchronization workflow.

Implementation workflows should not directly modify Canonical Knowledge.

---

## Principle 5

Documentation should remain stable.

Temporary planning information must not become permanent documentation.

---

## Principle 6

Documentation should be understandable by both humans and AI agents.

---

# 4. Canonical Knowledge

Repository documentation is the canonical source of implemented knowledge.

Documentation should describe:

- Product behavior
- Engineering architecture
- Operational procedures
- Repository workflows
- Repository standards

Documentation should not describe:

- Planning discussions
- Pull Request history
- Commit history
- Brainstorming
- Temporary implementation notes

---

# 5. Documentation Lifecycle

Documentation progresses through the following lifecycle.

```
Planning

↓

Implementation

↓

Validation

↓

Knowledge Synchronization

↓

Canonical Knowledge
```

Repository documentation is updated only during Knowledge Synchronization unless another approved workflow explicitly states otherwise.

---

# 6. Document Ownership

Every document has one primary owner.

Ownership determines long-term stewardship.

Ownership does not restrict contribution.

---

# 7. Document Placement

Every document has exactly one canonical location.

Documents must be placed according to repository architecture.

Moving documents between domains should be rare.

---

# 8. Cross References

Documentation should reference existing documents rather than duplicate content.

Cross references should be preferred over copy-and-paste.

---

# 9. Documentation Quality

Repository documentation should be:

- Accurate
- Complete
- Current
- Concise
- Consistent

Documentation should avoid:

- Ambiguity
- Contradictions
- Redundancy
- Dead links
- Stale information

---

# 10. Change Management

Documentation changes should:

- Preserve repository consistency.
- Preserve canonical knowledge.
- Remove obsolete information.
- Maintain valid cross references.

Documentation should evolve incrementally.

Large structural changes should be exceptional.

---

# 11. AI Compatibility

Documentation should be structured for deterministic navigation.

Documents should:

- Have a single responsibility.
- Use stable terminology.
- Follow consistent structure.
- Be independently understandable.
- Link to related documents rather than duplicate them.

---

# 12. Compliance

Repository documentation is compliant when:

- Repository Architecture is followed.
- Documentation Architecture is followed.
- This Documentation Standard is followed.
- Knowledge Synchronization has completed successfully.

---

# 13. Exceptions

Exceptions should be rare.

Any exception must:

- Be explicitly justified.
- Preserve repository consistency.
- Avoid introducing duplicate knowledge.

---

# 14. Related Documents

## Repository Constitution

- AGENTS.md
- Documentation Architecture
- Repository Structure

## Related Playbooks

- Knowledge Synchronization

## Related Standards

- Repository Standard
- Naming Standard
- Writing Standard
