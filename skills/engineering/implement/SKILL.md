---
name: implement
description: "Implement a piece of work based on a spec or set of tickets."
disable-model-invocation: true
---

Implement the work described by the user in the spec or tickets.

## Branch first

Before writing any code, create a feature branch for the work (named after the ticket/feature) and do ALL work on it. Never commit directly to `main` — the user reviews changes as a PR, and work on `main` cannot be reviewed that way. When the work is complete and reviewed, push the branch and open a PR (or ask the user how they want to review if no remote/tracker flow is configured).

## Tests

Use /tdd where possible, at pre-agreed seams.

Honor the /tdd **test-case review gate**: before any test is written, present the functionality under test and the proposed test cases (unit and e2e) and get the user's approval. Do not let implementation pressure skip this — no tests means no implementation.

Run typechecking regularly, single test files regularly, and the full test suite once at the end.

## Review

Once done, use /code-review to review the work.
