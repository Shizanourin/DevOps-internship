# Task 4 Summary: Mastering the Git Workflow

This document provides a concise breakdown of the actions taken to conquer **Task 4: Building a Version-Controlled DevOps Project**, focusing on implementing a professional and stable Git branching strategy.

---

## 1. Project Launch and Setup

The project started with foundational Git commands to establish a clean environment:

* **Repository Init:** Started a new project folder and initialized it with `git init`.
* **Initial Baseline:** Created the necessary starting files (like the `README.md`) and recorded them with the very first commit on the **`main`** branch.
* **Keeping it Clean:** Added a **`.gitignore`** file immediately to prevent logs, temporary files, and other junk from polluting the repository history.
* **Cloud Connection:** Linked the local repo to the remote GitHub location and published the `main` branch.

## 2. Establishing the Branch Structure

We set up a robust branching system to keep stable code separate from active development:

* **The Development Hub:** Created the **`dev`** branch directly from `main`. This branch is now the primary staging area where all new features are merged and tested before release.
* **Remote Synchronization:** Pushed the new `dev` branch to GitHub to make it available for the team.

## 3. Developing Features Safely

All new functionality was built in isolation, minimizing risk to the main development line:

* **Isolated Work:** A dedicated **`feature/add-script`** branch was spun off from `dev`. This is where all the coding for the new task happened.
* **Committing Progress:** Wrote a test script (`new_script.sh`) and committed the changes under this feature branch.
* **Sharing the Work:** Pushed the `feature/add-script` branch up to the remote for collaboration.

## 4. The Power of Pull Requests (PRs)

We used Pull Requests as a quality gate for all code integration:

* **Feature Review:** Created a **Pull Request** to move the finished code from **`feature/add-script` into `dev`**. This step is crucial—it's where code review happens and bugs are caught.
* **The Release Gate:** After successful testing in `dev`, a second, final **Pull Request** was created to merge **`dev` into `main`**. This formal step officially promotes the stable code to the production branch.

## 5. Marking the Release

To clearly identify the final, stable version of the code, we used a non-moving pointer:

* **Creating the Milestone:** On the final `main` branch, a **Git Tag** (a version label) was applied to permanently mark the exact point of the stable release.
* **Permanent Record:** Pushed the new tag to the remote repository.
* **Full Disclosure:** Ensured that a detailed `report.md` was updated with all the project steps and outcomes.
```eof
