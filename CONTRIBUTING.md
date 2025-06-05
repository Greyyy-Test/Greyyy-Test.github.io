# Contributing to LaMET Webpage

Thank you for your interest in contributing to the LaMET (Large Momentum Effective Theory) webpage! This guide explains how to collaborate via pull requests (PRs) while keeping our master branch clean and our work collaborative.

---

## 🛠️ How to contribute: step-by-step

1. **Clone** the repository to your local machine:
   ```bash
   git clone https://github.com/LaMET4Parton/LaMET4Parton.github.io.git
   cd LaMET4Parton.github.io
   ```
2. **Create a new branch** for your changes:
   ```bash
   git checkout -b your-feature-name
   ```
3. **Make your changes and commit:**
   ```bash
   git add .
   git commit -m "Brief description of your changes"
   git push origin your-feature-name
   ```
4. **Open a Pull Request (PR) on GitHub**, targeting the `master` branch.

5. **If you encounter a conflict** (e.g., GitHub shows a message like _"This branch has conflicts that must be resolved"_), click **Resolve conflicts**, then:
   - Delete the sections you don’t want to keep,
   - Keep the correct version of the content (usually from your PR branch),
   - Remove the conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`),
   - Then click **Mark as resolved** and **Commit merge**.

6. **Merge your PR:**
   - Use the **Squash and merge** button to keep commit history clean.
   - Edit the commit message to clearly summarize what the PR does.

7. **Delete your branch and update your local repository:**
   - On GitHub, after merging, click "Delete branch" to remove the feature branch from the remote.
   - On your local machine, switch to the `master` branch and pull the latest changes:
     ```bash
     git checkout master
     git pull
     ```
   - Delete your local feature branch:
     ```bash
     git branch -d your-feature-name
     ```
   - For next edits, repeat the process from step 2.
---

## 🛡️ Repository Rules

The following rules are enforced to ensure consistency and collaboration:

* **No direct push** to `master` allowed (everyone must use PRs)
* **Squash merge only** (each PR results in a single commit)
* **At least 0 approval** is required to merge a PR, so everyone can self-merge their own PRs
* **All code review comments must be resolved** before merging
* **Force pushes and branch deletions are blocked**

---

## 📘 Tips for Contributors

* Use descriptive commit messages like `Add Publications page` or `Fix layout bug in FAQ`
* Keep your PRs focused — small, clear, and reviewable
* You can collaborate on the same PR by pushing to a shared branch

---

## 🧑‍💼 Maintainers

* Admins may review and request changes
* Everyone with write access can submit PRs and self-merge
* Please be respectful and collaborative when reviewing others' work

---

Happy contributing! 🎉

If you have questions, open an issue or reach out in the collaboration channel. 