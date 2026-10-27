---
name: run-tests-on-code-change
description: Run the relevant automated tests after editing code or changing a function, and report the command and outcome.
---

# Run Tests On Code Change

Run tests after making code changes that can affect program behavior, including edits to functions, methods, modules, configuration that influences execution, or tests themselves. Do this in the same task before reporting completion; do not wait for the user to ask for verification.

Use repository instructions and project documentation to find the prescribed test command and working directory. Inspect relevant tests when needed to choose focused coverage. Run the smallest relevant test selection first when the project supports it; run the broader prescribed suite when the change can affect other behavior or project guidance requires it. Do not add dependencies or modify tests merely to make a test command easier to run.

If no automated tests exist, say so and use an appropriate non-destructive check when available. If tests cannot run because of a missing dependency, environment limitation, or another failure, report the exact command and blocker; do not claim the change is verified. If a test fails, investigate whether the failure relates to the change, fix it when within the requested scope, and rerun the relevant tests.

In the completion summary, state which tests were run and whether they passed. Keep test execution within the user's requested scope and existing repository guidance.
