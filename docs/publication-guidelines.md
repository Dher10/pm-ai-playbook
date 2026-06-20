# Publication Guidelines

This document defines the publication rules for the `pm-ai-playbook` repository.

The purpose of these guidelines is to ensure that prompts, workflows, templates, examples, and future AI agent concepts can be published safely as reusable Product Management knowledge.

This repository is public. Any content added here must be treated as public-facing material.

---

## Core Principle

Publish the pattern, not the private instance.

The repository should teach reusable Product Management methods, not expose internal product details, operating models, customer information, internal architecture, pricing, metrics, or proprietary workflows.

Before adding any content, ask:

```text
Does this teach a transferable pattern, or does it reveal an internal advantage?
```

If it reveals an internal advantage, do not publish it.

---

## What Can Be Published

The following types of content are generally safe to publish when written generically:

- reusable Product Management prompts
- prompt templates
- workflow patterns
- empty templates
- fictional examples
- generic quality checklists
- decision frameworks
- public-safe AI agent concepts
- general Product Management principles
- sanitized lessons learned

Content should be written so that another Product Manager could reuse it in a different company, product, or team.

---

## What Must Not Be Published

Do not publish:

- customer names
- employee names
- stakeholder names
- internal project names
- internal product names
- company-specific identifiers
- credentials or secrets
- API keys or tokens
- internal URLs
- private repository names
- endpoints
- system architecture details
- cloud account details
- infrastructure details
- internal pricing
- margins
- real commercial terms
- real usage metrics
- real roadmap commitments
- private backlog conventions
- real ticket identifiers
- real design file identifiers
- legal documents copied from internal sources
- internal screenshots
- proprietary operating procedures
- examples derived directly from private documents

When in doubt, remove, generalize, or keep the content internal.

---

## Public-Safe Abstraction Rules

When transforming internal knowledge into public content:

1. Replace real product names with generic descriptions.
2. Replace client or stakeholder names with neutral roles.
3. Replace real numbers with fictional or placeholder values.
4. Replace internal tools with generic tool categories.
5. Replace team-specific conventions with configurable inputs.
6. Convert real workflows into reusable patterns.
7. Avoid copying internal text verbatim.
8. Use fictional examples only.
9. Remove operational details that could reveal how the organization works internally.
10. Preserve the learning value while removing the private context.

Example:

```text
Do not publish:
"Create a Jira story using our DEV-FRONT prefix and assign it to the OWL product board."

Publish instead:
"Create a backlog item using the team's provided naming convention and label structure."
```

---

## Classification Model

Every new idea should be classified before being added to the repository.

Use one of the following classifications:

| Classification | Meaning | Publication Rule |
|---|---|---|
| Safe for public | The idea is generic and does not expose private context | Can be published |
| Public with abstraction | The idea is useful but comes from internal work | Must be generalized before publishing |
| Internal only | The idea depends on private systems, data, workflows, or operating advantage | Do not publish |

If an idea is classified as internal only, only a high-level public pattern may be documented, if it does not reveal sensitive operational detail.

---

## Prompt Publication Rules

Before publishing a prompt, verify that:

- the prompt solves a reusable Product Management problem
- the prompt does not include company-specific context
- the prompt does not hardcode private naming conventions
- the prompt does not depend on internal tools
- the prompt does not include real customer or stakeholder information
- the prompt uses configurable inputs when team-specific rules are needed
- the prompt includes a clear `When to Use` section
- the prompt states limitations or conditions where it should not be used
- the prompt includes validation rules
- the prompt prevents unsupported assumptions and invented information

Prompts should be useful without requiring access to internal systems.

---

## Workflow Publication Rules

Before publishing a workflow, verify that:

- the workflow describes a reusable process
- internal systems are described only as generic sources or tools
- real approval flows are not copied if they reveal internal operating models
- any connected-system behavior is abstracted
- all examples are fictional
- human approval points are clear
- risks and limitations are documented

If a workflow depends on a real tracker, repository, documentation corpus, or product system, publish only the pattern, not the integration.

---

## Template Publication Rules

Templates are usually safe to publish when they are empty and generic.

Before publishing a template, verify that:

- no real product information is included
- no real customer information is included
- no internal naming conventions are hardcoded
- no proprietary fields are exposed
- examples are fictional or omitted
- the template can be reused by another Product Manager

If a template originated from internal work, simplify it into a general-purpose structure.

---

## Example Publication Rules

Examples are the highest-risk part of the repository.

Before publishing an example, verify that:

- the product is fictional
- the company is fictional
- the users are fictional
- the data is fictional
- the metrics are fictional
- the roadmap is fictional
- the screenshots are not internal
- the wording is not copied from internal documents
- the example cannot be reverse-engineered into a real product or client

Prefer using one canonical fictional product across the repository to keep examples consistent and safe.

---

## AI Agent Publication Rules

AI agent concepts may be documented only when they are public-safe.

Do not publish agent implementations that connect to:

- live backlog systems
- private repositories
- internal documentation
- customer data
- production systems
- analytics platforms
- internal communication tools
- private design files

For public agent concepts, document only:

- purpose
- user
- trigger
- generic inputs
- expected outputs
- human approval points
- guardrails
- risks
- public vs. internal classification

Any agent that can read or write internal systems should remain internal.

---

## Human Approval Rules

For this repository, AI can assist with drafting, reviewing, and structuring content.

However:

- AI-generated content must be reviewed before publication.
- AI must not decide whether sensitive content is safe without human validation.
- AI-generated examples must be checked for accidental resemblance to real products.
- Any repository write should be explicit and scoped.
- Public-facing content must be reviewed for confidentiality, usefulness, and clarity.

---

## Pre-Publication Checklist

Before adding or updating any artifact, verify:

- [ ] The content is useful for Product Management.
- [ ] The content is reusable outside the original company or product.
- [ ] The content does not include real customer, employee, stakeholder, or product names.
- [ ] The content does not include credentials, endpoints, URLs, IDs, or private repository names.
- [ ] The content does not expose architecture, pricing, margins, or private metrics.
- [ ] The content does not hardcode internal naming conventions.
- [ ] The content uses fictional examples or no examples.
- [ ] The content teaches a pattern rather than revealing an internal advantage.
- [ ] The content is aligned with `docs/prompt-template.md` when it is a prompt.
- [ ] The content is aligned with `docs/prompt-quality-checklist.md` when it is a prompt.
- [ ] The content is aligned with this publication guide.

If any item fails, revise the content before publishing.

---

## Final Rule

When there is uncertainty, do not publish the detail.

Abstract it, remove it, or keep it private.

The value of this repository should come from clear Product Management thinking, reusable AI-assisted methods, and strong publication judgment.
