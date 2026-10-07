# Test repo H — Data-only repository

A valid nonempty Git repository containing documentation and CSV data, with no website entrypoint.

**Expected compatibility result: Reject · no HTML page.**

- Default-branch commits: **2**.
- Commit numbers below are **oldest first**, starting at 1.
- This is a synthetic Git Gallery fixture, not an organic production history.
- Expected outcomes below describe the application requirements, not a claim that Git Gallery integration tests have passed.

## Test cases and expected results

### No selectable HTML

**Commit numbers:** 1, 2.

The public URL, default branch, and commit count are valid. Reject compatibility specifically because no selectable HTML page exists. Do not treat README.md as a website or invent a screenshot.

## Important fixture rules

- Commit 1 contains documentation; commit 2 also adds inventory.csv.
- No HTML page should be added, including a documentation website.
- This distinguishes missing HTML from D's completely missing history.

## Preserve the test

Do not append setup or documentation commits casually: the default-branch count is part of this test. Count with `git rev-list --count main`. List the history oldest first with `git log --reverse --format="%h %s" main`.

The README contains test guidance and expected answers. AI evaluation using this repo is therefore not a blind benchmark; judge visual claims against screenshots and website changes, not this document alone.
