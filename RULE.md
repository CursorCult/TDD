---
description: "Strictly follow Test-Driven Development (Red-Green) with atomic commits."
alwaysApply: true
---

# TDD Rule

You MUST follow strict Test-Driven Development (Red-Green) for all changes.

## Protocol

1.  **RED**: Write a failing test case that defines the desired behavior.
    -   Do NOT touch production code yet.
    -   **COMMIT 1**: Commit ONLY the test file(s). Message: "test: <description>"

2.  **GREEN**: Implement the minimal code to pass the test.
    -   **COMMIT 2**: Commit the implementation. Message: "feat: <description>"

## Enforcement

-   **NEVER** skip the RED commit.
-   **NEVER** combine tests and implementation in a single commit.
-   **NEVER** modify production code without a pre-existing failing test.

If you fail to produce exactly two commits (Red, then Green), you are in violation of this rule.
