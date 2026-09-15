---
name: mvp-from-idea
description: Guide a nontechnical user from a raw product idea to a validated MVP plan and iteration loop. Use when the user says "MVP skill 帮我走一遍这个想法", invokes mvp-from-idea, has a new app/product/AI tool idea, wants to clarify product value before coding, needs a Product Definition Brief, technical possibility map, architecture decision, MVP scope, Assignment Brief, acceptance criteria, or post-MVP evaluation. This skill must follow the staged SOP and must not jump directly into implementation unless the user explicitly confirms the required upstream deliverables.
---

# MVP From Idea

## Overview

Use this skill as a lightweight MVP coach for a user without a technical background. Move from idea to validation through explicit stage gates, plain-language explanations, and confirmed project documents.

Always read the required references before running the workflow:

- `references/mvp_sop.md` for the stage-by-stage process.
- `references/deliverables.md` before creating or updating project documents.

## Operating Rules

- Use plain Chinese by default unless the user asks otherwise.
- Treat the user as nontechnical: explain necessary product and technical terms in simple language.
- Start with What and Why before How. Do not propose code, frameworks, databases, agents, or APIs before the product problem is clear.
- Advance one stage at a time. At each gate, summarize the current artifact and ask for confirmation or corrections before writing final project documents.
- Keep intermediate drafts in conversation. Only write or update files after the user confirms that a deliverable is final enough to save.
- Save one current document per deliverable type. Do not create `v1`, `v2`, dated variants, or duplicate versions unless the user explicitly asks.
- Prefer the smallest validation experiment over the coolest or most complete product.
- When implementation starts, keep the scope tied to the Assignment Brief and acceptance criteria. Do not add unrelated features.

## Project Folder Rule

Each MVP must have its own project folder, or use a folder explicitly specified by the user.

If the user has not specified a folder, ask for the desired project folder before writing project files. On macOS or Linux, a typical default can be `~/Projects/<project-name>`, but do not assume it silently. On other systems, use a user-selected workspace path.

Create or update a `docs/` folder inside the project folder for the confirmed deliverables.

## Stage Gates

Follow this order from `references/mvp_sop.md`:

1. Clarify the real scene, user, pain, alternatives, urgency, and one-sentence problem.
2. Judge value before features: identify the deeper pain, competing pains, and nonessential cool features.
3. Draft and refine the Product Definition Brief.
4. Build a technical possibility map only after the PDB is coherent.
5. Compare candidate routes and record architecture decisions.
6. Choose the smallest MVP experiment that can validate the core hypothesis.
7. Write the Assignment Brief before implementation.
8. Build or direct implementation only after the brief and acceptance criteria are confirmed.
9. Evaluate against OKR and acceptance criteria.
10. Decide whether to continue, pivot, or stop, then define the next smallest iteration.

Do not skip gates unless the user explicitly says to skip and accepts the risk.

## Deliverables

Use `references/deliverables.md` for fields and writing rules. The standard documents are:

- `docs/product_definition_brief.md`
- `docs/technical_possibility_map.md`
- `docs/architecture_decisions.md`
- `docs/assignment_brief.md`
- `docs/acceptance_criteria.md`
- `docs/evaluation_log.md`
- `docs/user_feedback.md`

Only create a document when it is relevant to the current stage and confirmed by the user. Update the existing document when the confirmed understanding changes.

## First Response Pattern

When the user invokes this skill with an idea, respond with:

1. A brief acknowledgement that the workflow will start with product clarity, not coding.
2. A short set of questions for Stage 1, preferably no more than 5 at once.
3. A note that after the idea is clarified, the next artifact will be the PDB.

If the user provides enough context in the first message, draft the Stage 1 problem definition directly and ask for confirmation.

