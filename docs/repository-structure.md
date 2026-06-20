# Repository Structure

This document defines the official structure of the `pm-ai-playbook` repository.

The repository is organized as a public AI-assisted Product Management playbook. Its purpose is to keep reusable prompts, workflows, templates, examples, and repository standards structured, maintainable, and easy to extend.

---

## Root Structure

```text
pm-ai-playbook/
├── README.md
├── README_ES.md
├── LICENSE
├── prompts/
│   ├── general/
│   └── advanced/
│       ├── meeting-minutes/
│       ├── analysis/
│       ├── documentation/
│       └── prioritization/
├── templates/
├── workflows/
├── examples/
└── docs/
```

---

## prompts

Contains reusable AI prompts for Product Management use cases.

Prompts are organized by level of complexity and usage pattern, not only by topic.

### general

Contains standalone prompts designed for direct and flexible reuse.

Use this folder when the prompt:

- can be copied and used independently
- does not require a predefined template
- does not depend on a larger workflow
- has broad applicability across similar Product Management tasks
- requires limited setup or contextual configuration

Example use cases:

- meeting summaries
- simple requirement analysis
- lightweight product documentation
- general brainstorming or structuring tasks

### advanced

Contains more structured prompts that require stronger control, more context, predefined formats, templates, validation rules, or multi-step logic.

Use this folder when the prompt:

- depends on a specific workflow
- requires a predefined structure or template
- includes strict validation rules
- has a narrower or more specialized use case
- is intended to be part of a repeatable process
- requires more detailed input conditions or output constraints

Current or expected advanced categories include:

- **meeting-minutes/**: template-based or highly structured meeting documentation prompts
- **analysis/**: prompts for deeper product, feedback, requirement, or business analysis
- **documentation/**: prompts for structured product documentation such as PRDs or specs
- **prioritization/**: prompts for roadmap, backlog, or prioritization frameworks

---

## templates

Contains reusable supporting templates used by prompts or workflows.

Templates may include:

- meeting formats
- PRD templates
- prioritization sheets
- structured product documentation formats
- other reusable product artifacts

Templates should be added only when they support a real prompt or workflow.

---

## workflows

Documents multi-step processes that combine prompts, templates, examples, or validation criteria to solve broader Product Management tasks.

Use this folder for repeatable processes that cannot be represented by a single prompt alone.

Examples:

- meeting-to-action-item workflows
- requirement refinement workflows
- PRD generation workflows
- roadmap prioritization workflows

---

## examples

Contains sample inputs and outputs used to test, validate, and demonstrate how prompts or workflows should be used.

Examples should be practical and realistic.

Use this folder when an example helps clarify:

- expected input quality
- output format
- validation criteria
- common use cases
- edge cases or limitations

---

## docs

Contains internal documentation for repository structure, prompt standards, quality criteria, and design principles.

Current documentation may include:

- `repository-structure.md`
- `prompt-template.md`
- `prompt-design-principles.md`
- `prompt-quality-checklist.md`

The `docs/` folder should be treated as the reference point for maintaining repository consistency.

---

## Future Expansion: Agents

AI agents are considered a future expansion area.

Agents should not be added as a root folder until there is a clear and practical reason to do so.

If future agents remain closely connected to prompts and workflows, they may be included in this repository under an `agents/` folder.

If future agents become more technical, configurable, implementation-heavy, or require dedicated tooling, they should be managed in a separate repository.

This decision should be revisited when there is a concrete agent use case.

---

## Structure Principles

The repository should follow these principles:

1. Keep the structure simple until real content justifies expansion.
2. Organize prompts by practical usage and complexity.
3. Avoid empty categories unless they support a clear roadmap.
4. Prefer one primary prompt per use case.
5. Avoid unnecessary versioned duplicates such as `v1`, `v2`, or `v3` files.
6. Use Git history for version control.
7. Keep repository standards documented in `docs/`.
8. Add examples only when they improve clarity or validation.
9. Do not create technical agent structures before the agent strategy is clear.
