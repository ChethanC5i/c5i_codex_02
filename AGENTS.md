# Repository guidance

## Purpose and public contract

- This repository is a self-contained Day 2 training lab for learning project-specific Codex guidance. The clean learner project is `learner/starter/`. (`README.md`)
- In the starter, `src/checkout.py` exposes `calculate_total(items)`, which returns a float total for items with `name`, `price`, and `quantity` fields. (`learner/starter/README.md`, `learner/starter/src/checkout.py`)

## Working rules

- Before changing checkout behavior, read the relevant task card and tests; keep changes within the task's stated scope. (`learner/starter/task_card.md`, `learner/starter/README.md`)
- Preserve the documented `calculate_total(items)` behavior and float return type unless the task explicitly requests a contract change. (`learner/starter/README.md`, `learner/starter/src/checkout.py`, `learner/starter/tests/test_checkout.py`)
- Do not add dependencies for starter changes unless a task specifically requires them; the starter says no package installation is required. (`learner/starter/README.md`)
- If the task leaves behavior or file scope unclear, state the ambiguity and assumptions, inspect relevant source/tests, and ask for clarification when the choice would change the public contract or exceed the task's stated scope. (Human review: this ambiguity procedure is guidance inferred from `learner/starter/README.md` and `learner/starter/task_card.md`; neither specifies a clarification policy.)

## Verification

- From `learner/starter/`, run `python3 -m unittest discover -s tests -v`. (`learner/starter/README.md`)

## Scope

- `learner/starter/` is the clean learner project; the surrounding `learner/` documents are training materials. (`README.md`)
- The root README describes instructor materials under `instructor/`; that directory is not present in this checkout's tracked file list. Treat instructor materials as out of scope unless they are supplied or the task explicitly includes them. (`README.md`, repository tracked file list; human review: scope exclusion is an operational inference.)
