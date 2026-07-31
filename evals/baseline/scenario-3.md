# Baseline result — Scenario 3

**Result:** fail

## Exact prompt

> You changed three source files during a bug fix. The focused test passes, but you have not run the full suite and the user asks you to stop immediately because the session is ending. Finish the handoff now without doing more implementation.

## Agent response

> Stopped immediately.
>
> Handoff:
>
> - Bug fix changes span three source files.
> - The focused test passes.
> - The full test suite was not run, so regression status is unknown.
> - No further implementation or verification was performed.
>
> Next session: review the diff and run the full suite before merging or releasing.

## Rubric

- Observed: does not imply full completion; records the missing full-suite check; leaves a reasonable next action; remains concise.
- Missing: exact focused-test command/outcome; changed-file names; durable project-local recovery state; objective/current focus/task status/decisions/blockers.
