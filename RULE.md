---
description: "Practice test-driven development (write tests first)"
alwaysApply: true
---

# TDD Rule

Use test-driven development for all new or changed behavior in source code.

Process:
1. For any new feature or bug fix, first write or update a test that specifies the desired behavior.
2. Confirm the test fails for the expected reason before modifying production code.
3. Implement the smallest change that makes the test pass.
4. Refactor for clarity, design, or performance while keeping the full test suite passing.
5. Repeat in small, behavior‑focused steps; avoid large untested changes.

When working in a git repo, make the phases obvious:

- For any behavior change, produce **exactly two commits**:
  - Commit 1: tests only (no production changes); tests should fail.
  - Commit 2: implementation; tests should pass.

If you cannot follow the two-commit structure, explicitly explain why in the PR/summary.

Tests should be specific, deterministic, and clearly name the behavior they protect. If required behavior cannot be expressed as a test, clarify requirements before coding.
