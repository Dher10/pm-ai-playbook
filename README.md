# AI Product Management Playbook

![AI](https://img.shields.io/badge/AI-Product%20Management-blue)
![Product Management](https://img.shields.io/badge/Product-Management-green)
![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![License](https://img.shields.io/badge/license-MIT-green)

Language: English | Spanish version available at: [README_ES.md](README_ES.md)

---

## Table of Contents

- [Overview](#overview)
- [Repository Structure](#repository-structure)
- [Language Handling](#language-handling)
- [Prompt Structure](#prompt-structure)
- [How to Use This Repository](#how-to-use-this-repository)
- [Documentation Standards](#documentation-standards)
- [Future Evolution](#future-evolution)
- [Commit Convention](#commit-convention)
- [Disclaimer](#disclaimer)
- [Inspiration and Resources](#inspiration-and-resources)
- [License](#license)

---

## Overview

This repository is a public AI-assisted Product Management playbook.

It is designed to organize reusable prompts, workflows, templates, examples, and supporting documentation for practical Product Management work.

The goal is to provide a structured and evolving toolkit that helps Product Managers use AI more consistently across common activities such as:

- meeting summaries
- product documentation
- requirement analysis
- PRD generation
- roadmap prioritization
- workflow structuring
- operational automation
- future AI-assisted product agents

Rather than being only a prompt collection, this repository is intended to work as a practical playbook for applying AI to Product Management tasks in a repeatable and maintainable way.

The content is developed from real Product Management practice, iterative prompt refinement, and structured documentation standards.

---

## Repository Structure

The repository is organized around reusable Product Management tools and workflows.

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

### prompts

Contains reusable AI prompts for Product Management use cases.

Prompts are organized into two main levels:

- **general/**: standalone prompts designed for direct, flexible reuse.
- **advanced/**: more structured prompts that may require additional context, templates, validation rules, stricter output control, or multi-step logic.

### templates

Contains reusable supporting templates used by prompts or workflows.

Examples may include meeting formats, PRD templates, prioritization sheets, or other structured product artifacts.

### workflows

Documents multi-step processes that combine prompts, templates, examples, or validation criteria to solve broader Product Management tasks.

### examples

Contains sample inputs and outputs used to test, validate, and demonstrate how prompts or workflows should be used.

### docs

Contains internal documentation for repository structure, prompt standards, quality criteria, and design principles.

---

## Language Handling

Prompts in this repository are written primarily in English for consistency, maintainability, and compatibility with most AI tools.

However, prompts must support multilingual inputs and outputs.

General rule:

- Spanish input → Spanish output
- English input → English output

If a template or predefined document format is provided, the original template language and structure must remain unchanged unless the prompt explicitly states otherwise.

This allows prompts to be reused across different working environments without maintaining separate prompt versions for each language.

---

## Prompt Structure

Prompts in this repository should follow a consistent structure to improve clarity, reuse, and maintainability.

The standard prompt structure is defined in `docs/prompt-template.md`.

A typical prompt should include:

- Prompt Title
- Purpose
- When to Use
- Inputs
- Language Handling
- Prompt Instructions
- Output Format
- Validation
- Change Log

This structure helps ensure that prompts are understandable, reusable, and easier to improve over time.

---

## How to Use This Repository

A typical usage flow is:

1. Identify the Product Management task you want to support with AI.
2. Go to the corresponding folder inside `prompts/`.
3. Decide whether the task requires a general prompt or an advanced prompt.
4. Copy the prompt and provide the required inputs.
5. Use any supporting template if needed.
6. Review the output against the validation rules included in the prompt.
7. Improve or adapt the prompt only when the use case requires it.

General prompts are useful when the task is flexible and does not require strict formatting or external templates.

Advanced prompts are useful when the task requires more control, a predefined structure, stronger validation, or integration into a larger workflow.

---

## Documentation Standards

Repository standards and governance are documented in the `docs/` folder.

Key documents include:

- `docs/repository-structure.md` — official repository structure and folder purpose.
- `docs/prompt-template.md` — standard structure for prompts.
- `docs/prompt-design-principles.md` — principles for creating clear and reusable prompts.
- `docs/prompt-quality-checklist.md` — checklist for reviewing prompts before adding or updating them.

The `docs/` folder should be treated as the reference point for keeping the repository consistent as it grows.

---

## Future Evolution

This repository is expected to evolve beyond individual prompts.

Future improvements may include:

- additional reusable prompts
- advanced Product Management workflows
- practical examples based on realistic inputs
- reusable templates for product artifacts
- product frameworks adapted for AI-assisted work
- structured AI agents for Product Management tasks

Agents are considered a future expansion area.

They may later be included in this repository if they remain closely connected to prompts and workflows. If they become more technical, configurable, or implementation-heavy, they may be managed in a separate repository.

The long-term goal is to build a practical AI-assisted Product Management playbook that can be used, reviewed, and extended by others.

---

## Commit Convention

This repository uses Conventional Commits to keep the change history readable and maintainable.

Common commit types include:

- `feat` — new prompt, workflow, template, or functional content.
- `fix` — correction of an issue.
- `docs` — documentation update.
- `refactor` — structural improvement without changing the core intent.
- `chore` — maintenance work.

Examples:

```text
feat: add meeting summary prompt
docs: update repository structure
refactor: improve prompt template
chore: rename repository references
```

---

## Disclaimer

This repository does not claim originality over all concepts, frameworks, or methodologies referenced.

The content combines:

- practical Product Management experience
- widely known product and delivery practices
- AI-assisted workflows
- iterative prompt refinement
- public learning from the broader product and AI community

The purpose of this repository is to organize practical working tools, not to claim ownership over concepts that are already part of the broader Product Management or AI ecosystem.

Users should review and adapt all outputs generated from these prompts before using them in professional, operational, or business-critical contexts.

---

## Inspiration and Resources

This repository was partially inspired by useful resources from the Product Management and AI community.

One relevant reference is:

https://github.com/deanpeters/product-manager-prompts/

Additional references may be added over time as the playbook evolves.

---

## License

This project is licensed under the MIT License.

See the [LICENSE](LICENSE) file for more details.
