# skills

My personal collection of agent skills, synced from my Cursor and Claude directories.

> [!NOTE]
> **I didn't write these skills.** I found them online, from blogs, GitHub repos, and people sharing their setups, and collected the ones I use. This repo is my source of truth for keeping them in sync across machines and tools. It isn't meant to show off or take credit. All credit goes to the original authors (for example, `retro` and `writing-for-agents` come from [Matt Pocock](https://github.com/mattpocock)).

## Skills

| Skill | What it does |
| --- | --- |
| `brainstorming` | Explores intent, requirements, and design before any creative or feature work |
| `generate-task-list` | Turns a PRD or feature request into a step-by-step implementation task list |
| `grill-me` | Interviews you about a plan or design until every branch is resolved |
| `improve-codebase-architecture` | Finds refactoring opportunities, focusing on testability and deeper modules |
| `make-quiz` | Creates a pop quiz on a codebase's style, functionality, and integrations, then grades it strictly |
| `retro` | Runs a retrospective on a coding session |
| `review-finding-fixes` | Works through code-review findings one at a time and updates the review doc |
| `scroll-stop-builder-skill` | Builds a scroll-driven video animation website from a video file |
| `scroll-stop-prompter` | Generates image and video prompts for scroll-stopping product content |
| `write-a-prd` | Writes a PRD through a user interview and codebase exploration |
| `writing-for-agents` | Guidelines for writing skills, `AGENTS.md`, and `CLAUDE.md` |

## Install a skill

```sh
npx skills@latest add kyratzakos/skills/write-a-prd
```

Swap `write-a-prd` for any skill name in the table above.
