# Git & GitHub Learning Journey

This repository documents a series of exercises designed to build fundamental Git and GitHub skills. Each exercise tackles a specific concept, from local repository management to advanced collaboration features.

---

## Exercise 1: Basic Git Setup & First Commit

**Objective:** To install Git, configure user identity, initialize a local repository, and make the first commit of a `README.md` file.

**Steps Taken:**

1.  Installed Git
2.  Configured global `user.name` and `user.email`.
3.  Created a new directory `git-exercise-repo` and navigated into it.
4.  Executed `git init` to initialize the repository.
5.  Created `README.md` with initial content.
6.  Used `git add README.md` to stage the file.
7.  Committed changes with `git commit -m "Initial commit: Add README.md"`.

**Learning:** Understood the core `init`, `add`, and `commit` workflow, and the importance of user configuration.

---

## Exercise 2: Understanding Git Status & Diff

**Objective:** To observe the state of the working directory and staging area, and identify changes between versions.

**Steps Taken:**

1.  Modified `README.md` by adding a new line.
2.  Ran `git status` to see unstaged changes.
3.  Used `git diff` to view detailed line-by-line differences.
4.  Staged `README.md` with `git add README.md`.
5.  Ran `git status` again to see staged changes.
6.  Used `git diff --staged` (or `git diff --cached`) to view staged changes.
7.  Committed the changes.

**Learning:** Gained clarity on the three states (working directory, staging area, repository) and how `git status` and `git diff` help navigate them.

---

## Exercise 3: Branching & Merging Basics

**Objective:** To create, switch between, and merge Git branches.

**Steps Taken:**

1.  Created a new branch: `git branch feature/new-content`
2.  Switched to the new branch: `git checkout feature/new-content`
3.  Made changes to `README.md` on the new branch and committed them.
4.  Switched back to `main`: `git checkout main`
5.  Merged the feature branch into `main`: `git merge feature/new-content`
6.  Deleted the feature branch: `git branch -d feature/new-content`

**Learning:** Understood the concept of independent development lines and how to integrate them.

---

## Exercise 4: Resolving Merge Conflicts

**Objective:** To practice identifying and resolving merge conflicts when changes in different branches overlap.

**Steps Taken:**

1.  Created `branch-A` and modified a specific line in `file.txt`. Committed.
2.  Switched to `main`, then created `branch-B`. Modified the *same* line in `file.txt`. Committed.
3.  Switched back to `main`. Merged `branch-A`.
4.  Attempted to merge `branch-B`, which resulted in a conflict.
5.  Manually edited `file.txt` to resolve the conflict markers.
6.  Staged the resolved file and committed the merge.

**Learning:** Learned to navigate Git's conflict markers and manually resolve conflicting code.

---

## Exercise 5: Working with Remote Branches

**Objective:** To push local branches to a remote repository and track them.

**Steps Taken:**

1.  Ensured `main` branch was pushed to `origin`.
2.  Created a new local branch `feature/remote-test`.
3.  Made a commit on `feature/remote-test`.
4.  Pushed the new branch to GitHub: `git push -u origin feature/remote-test`
5.  Verified the branch appeared on GitHub.

**Learning:** Solidified understanding of `git push -u` and how to manage branches across local and remote repositories.

---

## Exercise 6: Git Ignore & Best Practices

**Objective:** To prevent unwanted files from being tracked by Git using `.gitignore`.

**Steps Taken:**

1.  Created dummy files like `temp.log`, `output.txt`, and a `node_modules/` directory.
2.  Observed `git status` showing these as untracked.
3.  Created a `.gitignore` file.
4.  Added patterns (e.g., `*.log`, `output.txt`, `node_modules/`) to `.gitignore`.
5.  Observed `git status` no longer listing these files.
6.  Committed `.gitignore`.

**Learning:** Importance of `.gitignore` for a clean repository and avoiding unnecessary file tracking.

---

## Exercise 7: Git Log & History Inspection

**Objective:** To explore the commit history using various `git log` options.

**Steps Taken:**

1.  Used `git log` for a full history.
2.  Tried `git log --oneline --graph --all` for a condensed, graphical view of branches.
3.  Used `git log -p` to see patch details for each commit.
4.  Explored `git log --author="Your Name"` and `git log --since="2 weeks ago"`.

**Learning:** Gained proficiency in navigating and understanding the commit history efficiently.

---

## Exercise 8: Forking & Pull Requests (Basic)

**Objective:** To understand the basic workflow of contributing to an open-source project via forking and pull requests.

**Steps Taken:**

1.  **(Simulated)** Forked a dummy repository on GitHub (or used a peer's repo).
2.  Cloned the forked repository to local machine.
3.  Created a new branch for changes.
4.  Made a small, meaningful change and committed it.
5.  Pushed the branch to my forked repository on GitHub.
6.  Created a Pull Request from my forked repository back to the original (upstream) repository.
7.  **(Optional)** Reviewed the PR process on GitHub.

**Learning:** Understood the typical open-source contribution workflow and the role of forking and pull requests.

---

## Resources

* **Atlassian Git Tutorial:** [https://www.atlassian.com/git/tutorials](https://www.atlassian.com/git/tutorials)
* **Git Official Documentation:** [https://git-scm.com/doc](https://git-scm.com/doc)
* **GitHub Docs:** [https://docs.github.com/](https://docs.github.com/)

---

## License

This repository is provided for educational purposes.