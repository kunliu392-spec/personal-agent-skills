# MVP From Idea SOP

Use this reference as the authoritative workflow when the user invokes `mvp-from-idea`.

## Principle

Do not start with "how to build it." Start with "what is this" and "why is it worth doing."

For a nontechnical user, the agent's job is to help manage AI work:

- define the goal clearly;
- provide necessary context;
- map technical possibilities in plain language;
- make tradeoffs;
- create validation criteria;
- guide evaluation and iteration.

## Workflow Map

```text
Idea / pain
  -> clarify What and Why
  -> write Product Definition Brief
  -> create technical possibility map
  -> compare routes and make architecture decisions
  -> find the smallest MVP experiment
  -> write Assignment Brief
  -> build the first version
  -> evaluate against OKR and acceptance criteria
  -> iterate, pivot, or stop
```

## Stage 1: Clarify The Problem

Goal: Turn a vague idea into a real user problem.

Ask for or infer:

1. What real scene triggered the idea?
2. Who has the problem?
3. How is the problem solved today?
4. What is painful about the current solution?
5. What benefit would the user get if the problem were solved?
6. Is the problem high-frequency, low-frequency, or critical at specific moments?
7. Is it urgent, important, or only nice to have?

Output:

- possible real scenes;
- likely user;
- pain point;
- current alternatives;
- core value versus cool but nonessential features;
- one-sentence problem definition.

Gate: Do not move to features or technology until the problem definition is coherent.

## Stage 2: Judge Value Before Features

Goal: Find the deeper pain, not only the visible feature.

Analyze:

1. surface feature;
2. deeper user pain;
3. whether multiple pains are mixed together;
4. how product shape changes if a different pain is chosen;
5. which pain is worth validating first;
6. which features are cool but not required for the first MVP.

Gate: Select one primary pain for MVP validation.

## Stage 3: Product Definition Brief

Goal: Create the product north star before technical work.

The PDB must include:

1. product name;
2. core problem;
3. user and scenario;
4. current alternatives;
5. why now;
6. MVP definition;
7. OKR;
8. explicit non-goals;
9. core assumptions;
10. acceptance criteria.

PDB self-check:

- Can the product be explained in one sentence?
- Is the user clear?
- Is the first version clear and small?
- Are non-goals explicit?
- Are OKR and acceptance criteria evaluable?
- Can the PDB become context for future AI work?

Gate: If these are unclear, refine the PDB before technical mapping.

## Stage 4: Technical Possibility Map

Goal: Help a nontechnical user see possible implementation paths before choosing one.

Do not write code. Produce a table with:

1. possible implementation route;
2. required components such as web app, mobile app, browser extension, database, backend API, AI model, automation tool, spreadsheet, manual process, or fake data;
3. complexity: low, medium, high;
4. key risks;
5. fit for first MVP;
6. fit for future product;
7. plain-language explanation of technical terms;
8. recommended 2-3 technical questions to research next.

Decision criteria:

- Can it validate the core assumption?
- Is it simple enough?
- Is risk controllable?
- Can it produce a prototype quickly?

Gate: Do not choose a complex route only because it is cooler or more complete.

## Stage 5: Technical Research And Architecture Decision

Goal: Compare 2-3 candidate routes and pick the first MVP route.

Compare:

1. user workflow;
2. required components;
3. development difficulty;
4. reliability;
5. future extensibility;
6. fit for MVP;
7. biggest risks;
8. recommendation.

Explain architecture in plain language:

- what the user does;
- what frontend means and does;
- what backend means and does;
- what the AI model or AI agent does;
- where data comes from and goes;
- where failure is most likely;
- what a nontechnical product owner should watch.

Gate: Record the chosen route, rejected routes, tradeoffs, and reevaluation trigger.

## Stage 6: Find The Smallest MVP Experiment

Goal: Validate the core value with the smallest cost.

Ask:

```text
If all complexity that does not affect core value validation is removed,
what is the simplest experiment version?
```

Distinguish:

1. core value assumptions;
2. implementation shell or incidental complexity;
3. a 1-3 day MVP;
4. what can be simulated with a button, webpage, spreadsheet, manual step, fake data, or human-in-the-loop process;
5. complex features to postpone;
6. success and failure signals.

MVP self-check:

- validates core value;
- small enough;
- can be built quickly;
- avoids complex shells;
- creates clear feedback;
- teaches something even if it fails.

Gate: Choose the fastest credible validation, not the most complete product.

## Stage 7: Assignment Brief

Goal: Convert the PDB and MVP route into a concrete task brief for AI coding or implementation.

Include:

1. background;
2. build goal;
3. user flow;
4. feature scope;
5. explicit non-goals;
6. technical approach;
7. files to create or modify;
8. acceptance criteria;
9. risks;
10. recommended implementation order.

Gate: Do not start implementation until the Assignment Brief and acceptance criteria are clear.

## Stage 8: Build Or Direct The First Version

When implementation is requested:

1. restate the goal and scope;
2. list key uncertainties before acting;
3. implement the smallest viable version;
4. avoid unrequested features;
5. explain how to run and test;
6. self-check against acceptance criteria.

Gate: If the user has not confirmed implementation, keep the work at planning and documentation level.

## Stage 9: Evaluate Performance

Evaluate against PDB, OKR, and acceptance criteria.

Review:

1. whether it runs;
2. whether core flow works;
3. whether core value is validated;
4. which OKR are met or missed;
5. whether problems come from product definition, technical implementation, user experience, or excessive scope;
6. what must be fixed next;
7. what can wait;
8. the next smallest Assignment Brief.

Avoid vague advice such as "optimize experience." Convert feedback into specific next actions.

## Stage 10: Continue, Pivot, Or Stop

Use MVP feedback to decide:

- Continue: core assumption is validated and users see value.
- Pivot: some value exists, but the original pain, scenario, or route is wrong.
- Stop: the core assumption is not supported, or the cost is not justified.

Output a one-week executable plan if continuing or pivoting.

