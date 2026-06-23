# Prompt Design Principles

This document defines the core principles used to design prompts for the `pm-ai-playbook` repository.

The objective is to ensure prompts remain **clear, reliable, reusable, practical, maintainable, and safe to publish**.

This repository is not only a prompt collection. It is a public AI-assisted Product Management playbook. Prompts should therefore teach reusable Product Management patterns without exposing private product context, internal operating models, confidential examples, or company-specific conventions.

---

## 1. Clarity over complexity

Prompts should prioritize clarity.

Instructions must be:

- direct
- unambiguous
- easy to follow

Avoid overly long instructions or unnecessary context that does not contribute to the task.

A clear prompt usually produces better results than a complex one.

---

## 2. Define the Product Management purpose

Every prompt should clearly explain the Product Management activity it supports.

A prompt should answer:

- What problem does it solve?
- What artifact or output does it help produce?
- What Product Management workflow does it support?
- Why is the prompt useful?

Avoid prompts that are too generic to be actionable.

A good prompt should help a Product Manager perform a specific task more consistently.

---

## 3. Explain when to use the prompt

Every prompt should include a clear `When to Use` section.

This section should explain:

- the practical situation where the prompt should be used
- the type of task the prompt supports
- the expected input condition
- whether the prompt is general or advanced
- limitations or situations where the prompt should not be used

The goal is to help users decide whether the prompt fits their situation before running it.

---

## 4. Define the role when useful

When appropriate, the prompt should define the role the model must assume.

Example:

```text
You are an experienced Product Management assistant.
```

Role definition helps guide the reasoning style, vocabulary, and level of judgment expected from the model.

Do not overuse roles when the task is simple. The role should add useful context, not unnecessary formality.

---

## 5. Define the task clearly

Every prompt should clearly state:

- what the model must do
- what input it should use
- what type of output is expected
- what must not be done

Example:

```text
Analyze the meeting transcript and extract key decisions, confirmed commitments, and critical follow-up items.
```

Avoid vague instructions such as:

```text
Help with this document.
```

The task should be specific enough that another person could understand the expected output without additional explanation.

---

## 6. Structure the process

For complex tasks, instructions should be broken into logical steps.

Example:

```text
1. Analyze the input content.
2. Identify key information.
3. Organize the information clearly.
4. Generate the structured output.
5. Validate the result before finalizing.
```

Step-by-step instructions improve reliability and consistency.

However, avoid adding unnecessary steps when the task is simple.

---

## 7. Control the output structure

Prompts should clearly define how the output must be structured.

This may include:

- headings
- tables
- bullets
- required fields
- templates
- formatting rules
- delivery format

Example:

```text
Meeting Summary
Key Decisions
Confirmed Commitments
Pending Follow-up
```

When a template is provided, the model must follow the template exactly unless the user explicitly asks for a structural change.

Output control is especially important when the result will be copied into a business document, backlog item, roadmap, or stakeholder communication.

---

## 8. Support multilingual workflows

Prompts should support multilingual use cases by default.

Rules:

- Spanish input should generate Spanish output.
- English input should generate English output.
- If a template is provided, the template language and structure must be preserved.
- If the user explicitly requests a different output language, follow the user’s instruction.
- Section headings, table headers, and generated content should be consistent with the selected output language.

This makes prompts reusable across professional contexts without requiring duplicate versions.

---

## 9. Avoid hallucinations and unsupported assumptions

Prompts should explicitly instruct the model not to invent information.

A prompt should define what to do when information is:

- missing
- unclear
- contradictory
- only implied
- assumed by the user but not evidenced in the input

Example:

```text
Do not add information that is not present in the input. If information is missing, write `Not specified`.
```

If assumptions are allowed, they must be labeled clearly as assumptions.

This is critical for Product Management work because invented decisions, dates, owners, metrics, or commitments can create execution risk.

---

## 10. Include validation steps

Prompts should include a final validation stage when the task has business impact or structured output.

The model should verify:

- the required structure was followed
- the output language is correct
- the output contains only supported information
- missing information is marked correctly
- the result is useful for the intended Product Management task
- any template structure was preserved

Validation helps reduce incomplete, inconsistent, or misleading responses.

---

## 11. Design for reuse

Prompts should be written in a way that allows them to be reused across different contexts.

Avoid instructions that depend on:

- a single company
- a single client
- a single internal process
- a single product implementation
- a private naming convention
- a specific internal tool

When team-specific rules are needed, make them configurable inputs instead of hardcoding them.

Reusable prompts increase the long-term value of the playbook.

---

## 12. Publish the pattern, not the private instance

This repository should teach transferable Product Management patterns.

Prompts must not expose:

- private product details
- customer names
- stakeholder names
- internal architecture
- pricing or margins
- real business metrics
- private backlog conventions
- real ticket identifiers
- private repository names
- internal URLs or endpoints
- operational know-how that creates internal advantage

If a prompt idea comes from internal work, abstract it before publication.

The public version should explain the method without revealing the private instance.

---

## 13. Use fictional examples only

Examples are useful, but they are also high risk.

Any example included in a prompt should be fictional.

Examples should not be copied, paraphrased, or lightly disguised from real internal documents.

A safe example should use:

- fictional products
- generic roles
- fictional data
- neutral business contexts
- placeholder metrics
- no real identifiers
- no real screenshots

If an example could be reverse-engineered into a real product, client, process, or internal decision, do not publish it.

---

## 14. Separate public prompts from internal agents

Prompts in this repository should be usable without direct access to internal systems.

If an idea requires connection to:

- live backlog systems
- private repositories
- internal documentation
- customer data
- production systems
- analytics platforms
- internal communication tools
- private design files

then it should not be published as an implementation in this repository.

Only the public-safe concept, pattern, or guardrail model may be documented.

Agents that read from or write to internal systems should remain internal unless they are fully abstracted and non-operational.

---

## 15. Keep prompts maintainable

Prompts should remain easy to modify over time.

Avoid:

- excessive internal complexity
- repeated instructions
- conflicting rules
- unclear sections
- hidden dependencies
- too many tasks in one prompt

If a prompt becomes difficult to understand or maintain, simplify it or split it into:

- a smaller prompt
- a workflow
- a template
- an example

Maintainability is part of prompt quality.

---

## Final note

The goal of this repository is not to create perfect prompts.

The goal is to build a practical, public, and reusable AI-assisted Product Management playbook.

A strong prompt should be:

- useful
- understandable
- adaptable
- safe to publish
- grounded in real Product Management judgment
- abstracted enough to protect private context

The value of the playbook comes not only from the prompts themselves, but from the discipline used to decide what should be public, what should be abstracted, and what should remain internal.
