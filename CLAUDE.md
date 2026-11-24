# img-metrics-demo
Practice repo for an Issue -> PR -> review workflow.

## Workflow
- Never commit to main. Work only on the current feature branch.
- Before implementing, write plan.md, then stop. Do not ask for approval in chat:
  tell the user to review it with `/crit plan.md` and wait.
- plan.md is a scratch file: never commit it.
- Keep each change scoped to the linked Issue. Propose a new Issue for anything out of scope.
- Run `pytest -q` and `ruff check .` before saying a task is done.
- Use Conventional Commits (feat:, fix:, test:, docs:, chore:).
- After a crit review ends, stop any crit server you started.

## Code
- Python 3.11, numpy only. Package in `src/imgmetrics/`, tests in `tests/`.
- Public functions need type hints and docstrings.

## Shared machine rules
- CPU only. Never kill processes you did not start.
