# MVP Deliverables

Use this reference before creating or updating project documents.

## Document Policy

- Keep one current document per deliverable type.
- Do not create `v1`, `v2`, dated copies, or duplicate variants unless the user explicitly asks.
- Draft and revise in conversation first.
- Write or update files only after the user confirms the deliverable is ready to save.
- Store documents under the MVP project's `docs/` folder.
- If no MVP project folder is specified, ask for it before writing files.

## Standard Files

```text
docs/product_definition_brief.md
docs/technical_possibility_map.md
docs/architecture_decisions.md
docs/assignment_brief.md
docs/acceptance_criteria.md
docs/evaluation_log.md
docs/user_feedback.md
```

## product_definition_brief.md

Purpose: Product north star.

Required sections:

```markdown
# Product Definition Brief

## Product Name

## One-Sentence Problem

## User And Scenario

## Current Alternatives

## Current Friction

## Why Now

## MVP Definition

## OKR

## Non-Goals

## Core Assumptions

## Acceptance Criteria
```

## technical_possibility_map.md

Purpose: Compare possible implementation routes before committing.

Required sections:

```markdown
# Technical Possibility Map

## Context

## Route Comparison

| Route | Components | Complexity | Key Risks | MVP Fit | Future Fit |
| --- | --- | --- | --- | --- | --- |

## Plain-Language Terms

## Recommended Research Questions

## Recommended MVP Route
```

## architecture_decisions.md

Purpose: Record why a route was chosen and what was postponed.

Required format:

```markdown
# Architecture Decisions

## Decision 001: [Decision Title]

### Context

### Candidate Options

### Final Choice

### Why This Choice

### Tradeoffs

### Revisit When
```

Append new decisions as new sections in the same file.

## assignment_brief.md

Purpose: Give AI coding tools or agents a concrete implementation task.

Required sections:

```markdown
# Assignment Brief

## Background

## Build Goal

## User Flow

## Feature Scope

## Non-Goals

## Technical Approach

## Files To Create Or Modify

## Acceptance Criteria

## Risks

## Implementation Order
```

## acceptance_criteria.md

Purpose: Define how the MVP will be checked.

Required sections:

```markdown
# Acceptance Criteria

## Must Run

## Core Flow Tests

## Output Quality

## Error Handling

## Non-Goals To Protect

## Manual Test Checklist
```

## evaluation_log.md

Purpose: Track what happened after each run or iteration.

Required format:

```markdown
# Evaluation Log

## [Date] Evaluation

### Goal

### Test Results

### OKR Met

### OKR Missed

### Main Problems

### Next Smallest Change

### Deferred Issues
```

Append new evaluations to the same file.

## user_feedback.md

Purpose: Preserve real usage feedback, even if the only user is the owner.

Required format:

```markdown
# User Feedback

## [Date] Feedback

### Usage Scenario

### User Goal

### Friction

### Valuable Result

### Useless Or Weak Result

### User Words

### Product Judgment
```

Append new feedback entries to the same file.
