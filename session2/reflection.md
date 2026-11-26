# Session 2 Reflection
**Name:** Norman Yusoff (97640)

## Q1. How do Issues and pull requests together support change control?
Issues and pull requests work together to create an end-to-end audit trail for every modification in a project. An Issue documents the reason for a change along with its expected results and acceptance criteria, while the pull request links the actual code changes on a branch directly back to that Issue using keywords like `Closes #1`. This ensures no code is added without a documented purpose, a review checkpoint, and a permanent merge record.

## Q2. Why did the conflict in Part 4 happen, and how could a team reduce such conflicts?
The conflict in Part 4 happened because `branch-a` and `branch-b` both started from the same commit and modified the exact same line in `session2/conflict-demo.md` with different values (`staging` vs. `production`). Because Git cannot guess which value is correct, it paused the merge for a human to decide. Teams can reduce these conflicts by keeping branches short-lived, pulling from `main` frequently, and communicating clearly so two developers do not edit the same lines simultaneously.

## Q3. What would be lost if people merged straight into main without a pull request?
Merging straight into `main` without a pull request would eliminate the peer review stage, increasing the risk of introducing bugs, accidental secrets, or incomplete features into the stable codebase. It would also break traceability, as there would be no central discussion thread linking the code changes to the original Issue or showing who verified the acceptance criteria before release.
