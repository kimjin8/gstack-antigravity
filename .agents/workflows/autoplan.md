// turbo-all
# /autoplan: Auto-Review Eng Pipeline

Load identity: [persona-gstack-autoplan.md](file:///Users/kimjin/Library/CloudStorage/GoogleDrive-hongkimjin@gmail.com/My%20Drive/2026%20LLC/gStack-Antigravity/.antigravity/rules/persona-gstack-autoplan.md)

## Phase 0: Setup & Background
1.  **Detection:** Run `ls -t ~/.gstack/projects/*/ | head -1` (rebranded to workspace context).
2.  **Restore Point:** Backup the plan file to `/Users/kimjin/.gemini/antigravity/brain/` (or current project's context).
3.  **UI Scope:** Scan for `component`, `form`, `screen` to trigger Design Review.

## Phase 1: CEO Review (Strategy)
1.  **Analysis:** Auto-run all 10 CEO review sections from the rule.
2.  **Gate:** Prompt user to confirm premises.
    `AskUserQuestion: "Premises detected: [X, Y, Z]. Proceed?"`

## Phase 2: Design Review (UI)
1.  **Score:** Evaluate all 7 dimensions of the UX from the rule.
2.  **Logic:** Correct structural gaps autonomously based on Princple 5.

## Phase 3: Eng Review & Test Plan
1.  **Adversarial:** Run Codex architectural check (using Antigravity's inner agent).
2.  **Verification:** Build the test diagram mapping every new UX flow to a test case.
3.  **Backlog:** Update `TODOS.md` with P0/P1/P2 items.

## Completion
1.  **Gate:** Present approval gate with Taste Decisions.
2.  **Log:** Write the final result to the local project history.
