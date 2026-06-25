# Light Superpowers

Light Superpowers is a lightweight Codex workflow plugin for people who want the useful discipline of Superpowers without forcing full brainstorming, planning, TDD, subagent, or branch-completion ceremonies for small tasks.

## Install

Add this repository as a Codex plugin marketplace:

```powershell
codex plugin marketplace add eqa1231/light-superpowers --ref main
```

Then install the plugin:

```powershell
codex plugin add light-superpowers@light-superpowers
```

Open a new Codex thread after installation so the skill index refreshes.

## Use

Invoke the skill explicitly when you want a task-sized workflow:

```text
Use $light-superpowers and keep this task lightweight.
```

Useful prompts:

```text
Use $light-superpowers: make the smallest safe change and verify it.
```

```text
Use $light-superpowers instead of the full Superpowers workflow.
```

## What It Does

- Keeps small tasks small.
- Uses short plans only when the work needs them.
- Avoids full brainstorming, design-doc, subagent, worktree, and branch workflows unless the task is high risk or the user asks.
- Keeps verification, but scales it to the task.
- Leaves project-specific rules and repository guidance in charge.

## Repository Layout

```text
.agents/plugins/marketplace.json
plugins/light-superpowers/.codex-plugin/plugin.json
plugins/light-superpowers/skills/light-superpowers/SKILL.md
```
