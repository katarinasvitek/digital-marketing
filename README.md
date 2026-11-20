# digital-marketing

AI skills for everyday digital marketing work, built and maintained by Katarina Svitek.

Each skill is a folder with a `SKILL.md` file: plain-language instructions that an AI agent (Claude or any agent that supports skills) follows to do one marketing job well. The repo also keeps the reports those skills produce.

## Skills

| Skill | What it does |
|---|---|
| [cro-website](skills/cro-website/SKILL.md) | Reviews a landing page, pricing page, feature page or lead form across 7 conversion dimensions (value proposition, headline, CTA, visual hierarchy, trust, objections, friction). Returns quick wins, high-impact changes, A/B test ideas and copy alternatives. Includes detailed form CRO guidance and experiment ideas by page type. |

## Audits and reports

| Report | Skill | Date |
|---|---|---|
| [katarinasvitek.com CRO audit](audits/katarinasvitek-com-cro-audit.md) | cro-website | 20 Nov 2026 |

## Repo structure

```
digital-marketing/
├── README.md          # This file: overview and index of skills and reports
├── AGENTS.md          # Instructions for AI agents working in this repo
├── CLAUDE.md          # Points Claude to AGENTS.md
├── skills/
│   └── <skill-name>/
│       └── SKILL.md   # One folder per skill
└── audits/
    └── <site>-<type>-audit.md   # Reports produced by the skills
```

## How to use a skill

- **Claude (claude.ai or desktop app):** save the skill to your account, then ask for the job in plain words, for example "Why isn't this landing page converting? https://example.com".
- **Claude Code or other agents:** copy the skill folder into the agent's skills directory (for Claude Code, `.claude/skills/`).
- **Any chat AI:** paste the contents of `SKILL.md` into the conversation, then give it the page to review.

## Adding a new skill

1. Create `skills/<skill-name>/SKILL.md` with `name` and `description` frontmatter. Use a lowercase, hyphenated name.
2. Add a row to the Skills table above.
3. Commit and push straight to `main`.
