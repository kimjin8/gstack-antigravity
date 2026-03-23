# 🚀 gStack-Antigravity: The AI Founder's Toolkit

Welcome to the **Antigravity Port of gStack**. 

## 🤔 What is gStack?

Originally created by **Garry Tan (CEO of Y Combinator)**, **gStack** is a framework that encodes decades of Silicon Valley engineering excellence into AI personas. Instead of just "chatting with an AI," you are working with a team of hyper-specialized "Digital Staff" (CEOs, Lead Engineers, Designers) who know exactly how to brainstorm, build, and audit high-growth software.

**gStack-Antigravity** brings this entire professional brain trust into your local Google Antigravity environment—making it faster, private, and 100% focused on your "vibe coding" journey.

---

## Quick start

1. Install gStack-Antigravity (30 seconds — see below)
2. Run `/office-hours` — describe what you're building
3. Run `/plan-ceo-review` on any feature idea
4. Run `/review` on any branch with changes
5. Run `/qa` on your staging URL
6. Stop there. You'll know if this is for you.

## Install — 30 seconds

**Requirements:** [Antigravity](https://github.com/google-deepmind/antigravity), [Git](https://git-scm.com/), [Bun](https://bun.sh/) v1.0+, [Node.js](https://nodejs.org/) (Windows only)

### Step 1: Install on your machine

Open Antigravity and paste this. The agent does the rest:

> Install gStack-Antigravity: run **`git clone https://github.com/kimjin8/gstack-antigravity.git ~/.antigravity/skills/gstack && cd ~/.antigravity/skills/gstack && ./gstack-source/browse/setup`** then add a "gstack" section to your persona instructions that says to use the `/browse` skill from gstack for all web browsing, never use default browser tools, and lists the available skills: /office-hours, /plan-ceo-review, /plan-eng-review, /plan-design-review, /design-consultation, /review, /ship, /land-and-deploy, /canary, /benchmark, /browse, /qa, /qa-only, /design-review, /setup-browser-cookies, /setup-deploy, /retro, /investigate, /document-release, /codex, /cso, /autoplan, /careful, /freeze, /guard, /unfreeze, /gstack-upgrade. Then ask the user if they also want to add gstack to the current project so teammates get it.

### Step 2: Add to your repo so teammates get it (optional)

> Add gStack-Antigravity to this project: run **`cp -Rf ~/.antigravity/skills/gstack .antigravity/skills/gstack && rm -rf .antigravity/skills/gstack/.git && cd .antigravity/skills/gstack && ./gstack-source/browse/setup`** then add a "gstack" section to your project's `.antigravity/rules/persona-gstack.md` that says to use the `/browse` skill from gstack for all web browsing, never use default browser tools, lists the available skills: /office-hours, /plan-ceo-review, /plan-eng-review, /plan-design-review, /design-consultation, /review, /ship, /land-and-deploy, /canary, /benchmark, /browse, /qa, /qa-only, /design-review, /setup-browser-cookies, /setup-deploy, /retro, /investigate, /document-release, /codex, /cso, /careful, /freeze, /guard, /unfreeze, /gstack-upgrade, and tells the agent that if gstack skills aren't working, run `cd .antigravity/skills/gstack && ./gstack-source/browse/setup` to build the binary and register skills.

Real files get committed to your repo (not a submodule), so `git clone` just works. Everything lives inside `.antigravity/`. Nothing touches your PATH or runs in the background.

---

## 👀 See it work

```
You:    I want to build a daily briefing app for my calendar.
You:    /office-hours
AI:     [asks about the pain — specific examples, not hypotheticals]

You:    Multiple Google calendars, events with stale info, wrong locations.
        Prep takes forever and the results aren't good enough...

AI:     I'm going to push back on the framing. You said "daily briefing
        app." But what you actually described is a personal chief of
        staff AI.
        [extracts 5 capabilities you didn't realize you were describing]
        [challenges 4 premises — you agree, disagree, or adjust]
        [generates 3 implementation approaches with effort estimates]
        RECOMMENDATION: Ship the narrowest wedge tomorrow, learn from
        real usage. The full vision is a 3-month project — start with
        the daily briefing that actually works.
        [writes design doc → feeds into downstream skills automatically]

You:    /plan-ceo-review
        [reads the design doc, challenges scope, runs 10-section review]

You:    /plan-eng-review
        [ASCII diagrams for data flow, state machines, error paths]
        [test matrix, failure modes, security concerns]

You:    Approve plan. Exit plan mode.
        [writes 2,400 lines across 11 files. ~8 minutes.]

You:    /review
        [AUTO-FIXED] 2 issues. [ASK] Race condition → you approve fix.

You:    /qa https://staging.myapp.com
        [opens real browser, clicks through flows, finds and fixes a bug]

You:    /ship
        Tests: 42 → 51 (+9 new). PR: github.com/you/app/pull/42
```

You said "daily briefing app." The agent said "you're building a chief of staff AI" — because it listened to your pain, not your feature request. Eight commands, end to end. That is not a copilot. That is a team.

---

## 🏃 The sprint

gstack is a process, not a collection of tools. The skills run in the order a sprint runs:

**Think → Plan → Build → Review → Test → Ship → Reflect**

Each skill feeds into the next. `/office-hours` writes a design doc that `/plan-ceo-review` reads. `/plan-eng-review` writes a test plan that `/qa` picks up. `/review` catches bugs that `/ship` verifies are fixed. Nothing falls through the cracks because every step knows what came before it.

| Skill | Your specialist | What they do |
|-------|----------------|--------------|
| `/office-hours` | **YC Office Hours** | Start here. Six forcing questions that reframe your product before you write code. Pushes back on your framing, challenges premises, generates implementation alternatives. Design doc feeds into every downstream skill. |
| `/plan-ceo-review` | **CEO / Founder** | Rethink the problem. Find the 10-star product hiding inside the request. Four modes: Expansion, Selective Expansion, Hold Scope, Reduction. |
| `/plan-eng-review` | **Eng Manager** | Lock in architecture, data flow, diagrams, edge cases, and tests. Forces hidden assumptions into the open. |
| `/plan-design-review` | **Senior Designer** | Rates each design dimension 0-10, explains what a 10 looks like, then edits the plan to get there. AI Slop detection. Interactive — one AskUserQuestion per design choice. |
| `/design-consultation` | **Design Partner** | Build a complete design system from scratch. Researches the landscape, proposes creative risks, generates realistic product mockups. |
| `/review` | **Staff Engineer** | Find the bugs that pass CI but blow up in production. Auto-fixes the obvious ones. Flags completeness gaps. |
| `/investigate` | **Debugger** | Systematic root-cause debugging. Iron Law: no fixes without investigation. Traces data flow, tests hypotheses, stops after 3 failed fixes. |
| `/design-review` | **Designer Who Codes** | Same audit as /plan-design-review, then fixes what it finds. Atomic commits, before/after screenshots. |
| `/qa` | **QA Lead** | Test your app, find bugs, fix them with atomic commits, re-verify. Auto-generates regression tests for every fix. |
| `/qa-only` | **QA Reporter** | Same methodology as /qa but report only. Pure bug report without code changes. |
| `/cso` | **Chief Security Officer** | OWASP Top 10 + STRIDE threat model. Zero-noise: 17 false positive exclusions, 8/10+ confidence gate, independent finding verification. Each finding includes a concrete exploit scenario. |
| `/ship` | **Release Engineer** | Sync main, run tests, audit coverage, push, open PR. Bootstraps test frameworks if you don't have one. |
| `/land-and-deploy` | **Release Engineer** | Merge the PR, wait for CI and deploy, verify production health. One command from "approved" to "verified in production." |
| `/canary` | **SRE** | Post-deploy monitoring loop. Watches for console errors, performance regressions, and page failures. |
| `/benchmark` | **Performance Engineer** | Baseline page load times, Core Web Vitals, and resource sizes. Compare before/after on every PR. |
| `/document-release` | **Technical Writer** | Update all project docs to match what you just shipped. Catches stale READMEs automatically. |
| `/retro` | **Eng Manager** | Team-aware weekly retro. Per-person breakdowns, shipping streaks, test health trends, growth opportunities. `/retro global` runs across all your projects and AI tools (Claude Code, Codex, Gemini). |
| `/browse` | **QA Engineer** | Real Chromium browser, real clicks, real screenshots. ~100ms per command. |
| `/setup-browser-cookies` | **Session Manager** | Import cookies from your real browser (Chrome, Arc, Brave, Edge) into the headless session. Test authenticated pages. |
| `/autoplan` | **Review Pipeline** | One command, fully reviewed plan. Runs CEO → design → eng review automatically with encoded decision principles. Surfaces only taste decisions for your approval. |

### Power tools

| Skill | What it does |
|-------|-------------|
| `/codex` | **Second Opinion** — independent code review from OpenAI Codex CLI. Three modes: review (pass/fail gate), adversarial challenge, and open consultation. Cross-model analysis when both `/review` and `/codex` have run. |
| `/careful` | **Safety Guardrails** — warns before destructive commands (rm -rf, DROP TABLE, force-push). Say "be careful" to activate. Override any warning. |
| `/freeze` | **Edit Lock** — restrict file edits to one directory. Prevents accidental changes outside scope while debugging. |
| `/guard` | **Full Safety** — `/careful` + `/freeze` in one command. Maximum safety for prod work. |
| `/unfreeze` | **Unlock** — remove the `/freeze` boundary. |
| `/setup-deploy` | **Deploy Configurator** — one-time setup for `/land-and-deploy`. Detects your platform, production URL, and deploy commands. |
| `/gstack-upgrade` | **Self-Updater** — upgrade gstack to latest. Detects global vs vendored install, syncs both, shows what changed. |

---

## 🚀 10-15 Parallel Sprints

gstack is powerful with one sprint. It is transformative with ten running at once.

In the Antigravity environment, you can run multiple agent sessions in parallel — each in its own isolated workspace. One session on `/office-hours`, another on `/review`, a third implementing a feature, a fourth running `/qa`. All at the same time. The sprint structure is what makes parallelism work — without a process, ten agents is ten sources of chaos. With a process, each agent knows exactly what to do and when to stop.

---

## 📜 Credits & Recognition

This project is a localized port of the original **gstack** framework by **Garry Tan**. We are deeply grateful to Garry and the gstack team for their incredible work in building these powerful engineering personas.

*   **Original Source:** [garrytan/gstack](https://github.com/garrytan/gstack)
*   **Philosophy:** This port aims to make that same SV-level expertise accessible directly within the Google Antigravity environment, while keeping your work private and local.
