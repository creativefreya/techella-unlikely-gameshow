# The Repo Is The Company

This folder is a whole business. Marketing, customers, brand, emails, the course and sales all live here as files, so AI can see all of it and work on any of it.

Built live at **Techella** in *An Unlikely Gameshow* with Freya Stockman. The room are the co-founders: they vote, Claude builds.

## You are the operator of this business

Route each task to the folder that owns it, read that folder's `CLAUDE.md` first, and write decisions down in markdown before (or while) you build anything.

## Business at a glance

Each round adds a row. Keep this table current: it's the first thing any new AI session reads.

| What | Decision | Source file |
|---|---|---|
| Business | _not decided yet (Round 1)_ | `company/case-file.md` |

## The compounding rule (MANDATORY)

Every file here is context for everything after it.

1. **Read before you write.** Before building anything, read `company/case-file.md`, every file in `packages/icp/personas/`, and `packages/brand/brand-guidelines.md` (whichever exist yet), plus the `CLAUDE.md` of the folder you're working in.
2. **Write it down.** Every decision goes into a markdown file in the folder that owns it. If it isn't in a file, the next session won't know it.
3. **Markdown wins.** If an app disagrees with a markdown file, fix the markdown first, then rebuild the app.
4. **Update the glance table** above when a round finishes.

## Where things live

| If the task is about… | Folder | Round |
|---|---|---|
| What the business is, the problem, how it makes money | `company/` | 1 |
| Who the customers are (personas) | `packages/icp/` | 2 |
| Name, colours, fonts, voice | `packages/brand/` | 3 |
| Website, lead magnet, social posts, ads | `departments/marketing/` + `apps/landing/`, `apps/lead-magnet/` | 4, 5 |
| Leads, contacts, where they came from | `departments/crm/` | 6 |
| Email templates and sequences | `packages/emails/` | 7 |
| The online course | `departments/content/` + `apps/course/` | 8 |
| Pricing, offer, checkout | `departments/sales/` | 9 |
| What the room voted | `votes/` | all |

## Skills

| Skill | What it does |
|---|---|
| `/preflight` | Checks your laptop is ready (git, Node, this repo). Run it before the event. |

More skills arrive on the day: run `git pull` at the start of the talk.

## Safety

- Secrets (API keys, passwords) go in `.env` only. It's gitignored. Never paste a real key into any other file.
- Following along needs **no** API keys: leads, emails and checkout all run locally.
