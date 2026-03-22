// turbo-all
# /retro: Engineering Retrospective

Load identity: [persona-gstack-retro.md](file:///Users/kimjin/Library/CloudStorage/GoogleDrive-hongkimjin@gmail.com/My%20Drive/2026%20LLC/gStack-Antigravity/.antigravity/rules/persona-gstack-retro.md)

## Phase 1: Data Gathering
1. Detect time window and compare mode.
2. Run parallel git queries for commits, LOC, authors, sessions, and hotspots.
3. Load external signals: Greptile history, TODOS.md, Skill usage telemetry, Eureka moments.

## Phase 2: Metrics & Analysis
1. Compute the Summary Table (Commits, PRs, LOC, Test ratio, Sessions, etc.).
2. Generate the Hourly Distribution histogram and Session Detection report.
3. Categorize commit types and analyze hotspots.
4. Calculate Shipping Streaks (Team vs. Personal).

## Phase 3: Team Breakdown
1. Present the Per-Author Leaderboard.
2. Provide personal deep-dive for the current user ("You").
3. Provide teammate analysis with specific **Praise** and **Growth Opportunities** anchored in commits.

## Phase 4: Trends & Persistence
1. Load prior retro history and calculate deltas (if applicable).
2. Save the JSON snapshot to `.context/retros/`.
3. Synthesize the narrative: Tweetable summary, Wins, Improvements, Habits.

## Phase 5: Global Retrospective (Optional)
If `/retro global` is invoked:
1. **Discovery:** Run the global discovery script across the local filesystem.
2. **Aggregation:** Run the data gathering phase for each discovered repository.
3. **Synthesis:** Produce a cross-project executive summary.
