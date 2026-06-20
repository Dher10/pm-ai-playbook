# Prompt Quality Checklist

This checklist helps validate prompts before adding or updating them in the `pm-ai-playbook` repository.

The objective is to ensure prompts remain **clear, reliable, reusable, practical, and safe to publish**, while avoiding unnecessary complexity, ambiguity, or exposure of private context.

Before committing a new or updated prompt, review the following points.

---

## 1. Clarity

- [ ] The prompt clearly states what the model must do.
- [ ] Instructions are direct and easy to understand.
- [ ] There are no ambiguous or vague instructions.
- [ ] The prompt avoids unnecessary jargon unless the target user needs it.

Example of vague instruction:

```text
Help with this document.
```

Better instruction:

```text
Analyze the document and extract the key decisions, open questions, and follow-up actions.
```

---

## 2. Purpose

- [ ] The prompt clearly defines the purpose of the task.
- [ ] The expected outcome is easy to understand.
- [ ] The prompt explains what Product Management activity it supports.
- [ ] The prompt solves a reusable problem, not a one-off private scenario.

The reader should immediately know what the prompt is designed to produce and why it is useful.

---

## 3. When to Use

- [ ] The prompt includes a clear `When to Use` section.
- [ ] The section explains the practical situation where the prompt should be used.
- [ ] The section identifies the type of task the prompt supports.
- [ ] The section defines the expected input condition.
- [ ] The section states whether the prompt is general or advanced.
- [ ] The section explains any limitation or scenario where the prompt should not be used.

A good `When to Use` section helps users decide whether the prompt fits their situation before running it.

---

## 4. Folder Fit

- [ ] The prompt belongs in the correct folder.
- [ ] `prompts/general/` is used for standalone, flexible, reusable prompts.
- [ ] `prompts/advanced/` is used for prompts that require stricter structure, more context, templates, validation rules, or multi-step logic.
- [ ] The folder choice is consistent with the `When to Use` section.
- [ ] The prompt does not require a new folder unless there is a clear repeated use case.

If the prompt requires a specific workflow, template, or strong validation logic, it probably belongs in `prompts/advanced/`.

---

## 5. Input Definition

- [ ] The prompt clearly defines the required inputs.
- [ ] Optional inputs are marked clearly.
- [ ] Inputs are described in a way that avoids confusion.
- [ ] The prompt does not assume access to internal systems.
- [ ] Team-specific rules are passed as configurable inputs, not hardcoded.

Examples of inputs:

- meeting transcript
- product context
- user story
- template document
- supporting data
- team naming convention
- additional instructions

---

## 6. Structured Instructions

- [ ] The task is structured into logical steps when needed.
- [ ] The instructions guide the model through the task clearly.
- [ ] The prompt separates task instructions from output requirements.
- [ ] The prompt includes rules and constraints when needed.
- [ ] The prompt avoids overloading the model with unnecessary context.

Example:

```text
1. Analyze the provided content.
2. Identify key information.
3. Organize the output.
4. Validate the result before finalizing.
```

---

## 7. Output Structure

- [ ] The prompt defines the expected output structure.
- [ ] Sections or headings are clearly defined.
- [ ] Tables, bullets, or formats are specified when needed.
- [ ] The output format is practical for the intended user.
- [ ] If a template is provided, the prompt instructs the model to preserve the template structure exactly.

Example:

```text
Meeting Summary
Key Decisions
Action Items
Open Questions
```

---

## 8. Multilingual Handling

- [ ] The prompt supports multilingual inputs.
- [ ] The output language matches the input language.
- [ ] Spanish input generates Spanish output.
- [ ] English input generates English output.
- [ ] Templates preserve their original language and structure.
- [ ] The prompt explicitly states what to do if the user requests a different output language.

Prompts should support multilingual workflows by default unless there is a clear reason not to.

---

## 9. Hallucination Control

- [ ] The prompt explicitly prevents the model from inventing information.
- [ ] The prompt explains what to do when information is missing.
- [ ] The prompt explains what to do when information is unclear.
- [ ] Assumptions are labeled as assumptions when they are allowed.
- [ ] The prompt avoids creating unsupported metrics, dates, commitments, or decisions.

Example rule:

```text
Do not generate information that is not present in the input. If information is missing, write `Not specified`.
```

---

## 10. Validation Step

- [ ] The prompt includes a validation stage before final output.
- [ ] The model verifies structure, language, and completeness.
- [ ] The model checks that no unsupported assumptions were added.
- [ ] The model checks that template structure was preserved when a template is provided.
- [ ] The model checks that the output is useful for the intended Product Management task.

Example validation rule:

```text
Before finalizing, verify that the output follows the required structure, matches the input language, and does not include invented information.
```

---

## 11. Reusability

- [ ] The prompt can be reused in different scenarios.
- [ ] Instructions are not overly dependent on a single company, product, or team.
- [ ] Organization-specific rules are configurable.
- [ ] The prompt teaches a reusable Product Management pattern.
- [ ] The prompt can be understood without private context.

Reusable prompts increase the long-term value of the playbook.

---

## 12. Simplicity

- [ ] The prompt avoids unnecessary complexity.
- [ ] Instructions are as simple as possible while remaining effective.
- [ ] The prompt does not include redundant rules.
- [ ] The prompt does not try to solve too many tasks at once.
- [ ] If the prompt is becoming too broad, it can be split into smaller prompts or a workflow.

If a prompt feels overly complicated, it should probably be simplified.

---

## 13. Public Safety

- [ ] The prompt does not include real customer names.
- [ ] The prompt does not include employee or stakeholder names.
- [ ] The prompt does not include internal product names.
- [ ] The prompt does not include credentials, endpoints, URLs, IDs, or private repository names.
- [ ] The prompt does not expose architecture, pricing, margins, or private metrics.
- [ ] The prompt does not hardcode internal naming conventions.
- [ ] The prompt does not reproduce internal documents.
- [ ] The prompt uses fictional examples or no examples.
- [ ] The prompt teaches a pattern rather than revealing an internal advantage.

If any of these checks fail, revise the prompt before publishing it.

---

## 14. Examples

- [ ] Any example included in the prompt is fictional.
- [ ] The example cannot be reverse-engineered into a real product, customer, stakeholder, or internal process.
- [ ] The example supports understanding without exposing private context.
- [ ] The example uses generic roles and neutral product descriptions.
- [ ] The example avoids real metrics, real roadmap commitments, or real operational details.

Examples are useful, but they are also one of the highest-risk parts of a public repository.

---

## 15. Final Check Before Commit

Before committing a prompt to the repository, verify:

- [ ] The prompt follows `docs/prompt-template.md`.
- [ ] The prompt is aligned with `docs/publication-guidelines.md`.
- [ ] The prompt has a clear purpose.
- [ ] The prompt has a clear `When to Use` section.
- [ ] The prompt defines required and optional inputs.
- [ ] The prompt includes structured instructions.
- [ ] The prompt defines the expected output format.
- [ ] The prompt supports multilingual handling.
- [ ] The prompt includes hallucination-control rules.
- [ ] The prompt includes a validation step.
- [ ] The prompt is reusable.
- [ ] The prompt is safe to publish.
- [ ] The prompt is in the correct folder.

If all items are satisfied, the prompt is ready to be added or updated.
