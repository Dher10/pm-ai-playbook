# Prompt Template

This document defines the standard structure used to write prompts in this repository.

The objective is to keep prompts **clear, reusable, practical, and consistent**, while avoiding unnecessary complexity.

Version control, authorship, and dates are handled directly by GitHub.

---

## Prompt Title

Provide a clear and descriptive name for the prompt.

The title should describe the task or outcome the prompt supports.

Example:

```text
Meeting Summary from Transcript
```

---

## Purpose

Explain briefly what the prompt is designed to do.

This section should answer:

- What problem does the prompt solve?
- What output should be generated?
- What Product Management activity does it support?

Example:

```text
Generate a structured meeting summary from a meeting transcript, including key discussion points, decisions, action items, and open questions.
```

---

## When to Use

Explain the practical situation where the prompt should be used.

This section helps users decide whether the prompt is appropriate for their use case.

Include:

- the type of task the prompt supports
- the expected input condition
- whether the prompt is general or advanced
- any limitation or scenario where the prompt should not be used

Example:

```text
Use this prompt when you have a meeting transcript and need to convert it into a structured summary.

This is a general prompt when no predefined template is required.
Use an advanced prompt instead if the output must follow a strict client, company, or spreadsheet template.
```

---

## Inputs

Describe the inputs required to use the prompt.

Inputs should be specific enough for another person to understand what information must be provided.

Examples:

- Meeting transcript
- Supporting documentation
- Template to populate
- Additional instructions
- Product context
- Business rules or constraints

If an input is optional, mark it clearly.

---

## Language Handling

Prompts must support multilingual workflows.

Rules:

- The output language must match the language of the input content.
- Spanish input must generate Spanish output.
- English input must generate English output.
- If a template is provided, its language and structure must not be modified.
- Generated content must follow the language of the source material unless the prompt explicitly says otherwise.

Examples:

```text
Spanish transcript → Spanish output
English transcript → English output
```

---

## Prompt Instructions

Write the actual prompt instructions here.

A good prompt should include:

1. Role definition
2. Task description
3. Processing steps
4. Output requirements
5. Rules and constraints

Example structure:

```text
You are an expert Product Management assistant.

Your task is to analyze the provided input and generate structured output.

Steps:

1. Analyze the provided content.
2. Identify the most relevant information.
3. Organize the information clearly.
4. Follow the required output structure.

Rules:

- Do not modify the template structure if one is provided.
- Do not invent information that is not present in the input.
- Ensure clarity, completeness, and practical usefulness.
```

---

## Output Format

Define the expected output structure.

The output format should be explicit enough to reduce ambiguity.

Examples:

```text
Meeting Summary
Key Discussion Points
Decisions
Action Items
Open Questions
```

If a template is provided, the output must follow the template structure exactly.

---

## Validation

Before producing the final output, verify that:

- The structure follows the required format.
- The language matches the source input.
- The template structure has not been modified.
- All relevant information has been captured.
- No unsupported assumptions or invented information were added.
- The output is clear and usable for the intended Product Management task.

If any issues are detected, correct them before generating the final output.

---

## Change Log

Use this section to document meaningful updates to the prompt.

Use Git history as the primary source of version control. The change log should only capture meaningful structural or functional prompt changes.

| Version | Description |
|--------|-------------|
| v2.1 | Added When to Use section and clarified prompt structure expectations |
| v2.0 | Simplified prompt template structure and added multilingual handling guidelines |
| v1.0 | Initial prompt template |
