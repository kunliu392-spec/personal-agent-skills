# Personal Agent Skills

Private source repository for reusable Agent Skills.

## Included skills

- `mvp-from-idea`: Guides a nontechnical user from a raw product idea to a validated MVP plan and iteration loop.

## Codex installation

Clone this repository, then link the skill into the user-level Agent Skills directory:

```bash
mkdir -p ~/.agents/skills
ln -s ~/agent-skills/skills/mvp-from-idea ~/.agents/skills/mvp-from-idea
```

If the skill does not appear in Codex, restart Codex and invoke it explicitly with `$mvp-from-idea`.

