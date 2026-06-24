# Version Control Simulation — Project Reflection

**Name:** Kalabe Kebede  
**Date:** 2026-06-24  
**Repository:** https://github.com/Kalab21/version-control-simulation-kalabe

---

## 1. Creating and Managing Branches

The first step was creating a GitHub repository named `version-control-simulation-kalabe` and cloning it locally. From there, I created a `feature/header` branch using `git checkout -b feature/header`. This branch held the initial HTML structure, including a header element with a navigation menu containing Home, About, and Contact links. After staging and committing those changes, I switched back to the main branch and created a second branch called `feature/footer`. On this branch, I added a footer element with copyright information and a contact email. Each branch was kept focused on a single feature, which reflects real-world best practices where developers isolate their work to avoid disrupting the main codebase.

## 2. Handling the Merge Conflict

To simulate a conflict, I switched back to `feature/header` and added a different version of the footer section — a line that conflicted with what `feature/footer` had already written. I then merged `feature/footer` into `main` first, which succeeded cleanly. When I attempted to merge `feature/header` into `main`, Git detected a conflict in the footer section of `index.html` and marked it with conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`). I resolved the conflict by opening the file, removing the markers, and keeping the correct footer content from `feature/footer`. After saving, I staged the resolved file with `git add index.html` and committed the merge. This process taught me to carefully read conflict markers and make deliberate decisions about which changes to keep rather than blindly accepting one side.

## 3. Pull Requests and Code Quality

After pushing the resolved `main` branch to GitHub, I created a pull request from `main` into a `review/main` branch. The PR included a description of all changes made, a summary of the conflict resolution, and a test checklist. This process reinforced how pull requests serve as a quality gate — they give collaborators visibility into what changed and why, enable line-by-line code review, and create a documented history of decisions. Reviewing a peer's pull request further highlighted how a second set of eyes catches issues that the original author may overlook. Overall, this simulation demonstrated that version control is not just about saving code — it is a structured workflow that supports collaboration, accountability, and code quality across teams.
