# An Unlikely Gameshow — build a business in under 90 minutes with AI

Starter repo for Freya Stockman's talk at **Techella**. The room picks a business, votes on every big decision, and Claude Code builds it live: problem → customers → brand → website → lead magnet → CRM → emails → course → checkout.

You can just watch and vote on your phone. If you want to build along (or redo it at home), this repo is everything you need.

## Before the event

Follow [PREP.md](PREP.md), then open this folder in Claude Code and type:

```
/preflight
```

Green ticks = you're ready.

## On the day

```bash
git pull
```

This gets the round skills and the room's votes as they happen.

## The idea: the repo is the company

Most small businesses run on 8+ disconnected apps. None of them know about each other, so AI can't see the whole business either.

Here, every department is a folder. Every decision is a markdown file. Each round reads the files before it, so the business **compounds**: by the time we write the welcome emails, Claude already knows the customer's 2am worry, the brand voice and the lead magnet they downloaded.

## Round → file map

| Round | Name | Skill | Writes |
|---|---|---|---|
| 1 | The Case | `/case-file` | `company/case-file.md` |
| 2 | The Client | `/client-profile` | `packages/icp/personas/client.md`, `referral-partner.md`, `student.md` |
| 3 | Name That Brand | `/brand-kit` | `packages/brand/brand-guidelines.md`, `tokens.json` |
| 4 | Front Door | `/landing-page` | `departments/marketing/website.md`, `apps/landing/` |
| 5 | The Bait | `/lead-magnet` | `departments/marketing/lead-magnet.md`, `apps/lead-magnet/` |
| 6 | The Little Black Book | `/crm-connect` | `departments/crm/CLAUDE.md`, leads store |
| 7 | You've Got Mail | `/email-sequence` | `packages/emails/welcome-sequence.md` |
| 8 | Detective School | `/course-platform` | `departments/content/curriculum.md`, `apps/course/` |
| 9 | Show Me the Money | `/checkout` | `departments/sales/offer.md` |

Skills for rounds 1–9 land on the day via `git pull`.

## Folder structure

```
CLAUDE.md            ← the business's memory: AI reads this first
company/             ← what the business is (Round 1)
packages/
  icp/personas/      ← who we serve (Round 2)
  brand/             ← how we look and sound (Round 3)
  emails/            ← email templates (Round 7)
departments/
  marketing/         ← website + lead magnet plans (Rounds 4–5)
  crm/               ← leads and contacts (Round 6)
  content/           ← the course (Round 8)
  sales/             ← the offer and checkout (Round 9)
apps/                ← the pages people actually see
votes/               ← what the room voted, per round
```

## Want to take it further?

- **Got a business or an idea you want to run with AI?** [Book a free intro call with Freya](https://calendar.app.google/4KvK9MxbF5WkVN3g8). Talk it through and see a demo of the Company OS web app.
- **Want agents to run it for you?** That's the next step after today: see the end of the talk.
