---
name: create-skill
description: "Use this skill to create a new VS Code Copilot skill (`SKILL.md`) for the repository, with a clear name, description, and workflow guidance."
---

# Create Skill

This skill helps you generate a new Copilot skill file (`SKILL.md`) for a workspace or user prompt customization.

## What it produces

- A `SKILL.md` file with YAML frontmatter and a clear `description`.
- A concise skill name and statement of purpose.
- Guidance on the workflow, including steps, decision points, and expected outcomes.
- Suggestions for follow-up customizations when relevant.

## When to use it

- You want a new workspace or personal skill that encapsulates a multi-step workflow.
- You need a skill that can be discovered by Copilot via a meaningful `description`.
- You want to capture a repeatable process with clear criteria and completion checks.

## How to use it

1. Choose a skill name that describes the workflow, for example `java-coding-skill` or `new-java-e2e-test-yaml-and-test`.
2. Provide a short, specific description of what the skill does and when it applies.
3. Describe the step-by-step process the skill should follow.
4. Include any decision logic, quality checks, or guardrails needed for the workflow.
5. Place the skill under `.github/skills/<skill-name>/SKILL.md`.

## Example prompt

"Create a new Copilot skill for validating API schema changes in `go/` and adding a test harness sample."

## Suggested next steps

- Add a matching prompt file if the workflow needs structured user inputs.
- Add an instruction file if the guidance should apply to all repository edits in a specific area.
- Add a custom agent if the workflow requires isolated tool restrictions or staged context handling.
