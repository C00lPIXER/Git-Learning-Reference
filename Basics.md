```markdown
# Git Basics

## What is Git?

<!-- 
Git is a distributed version control system (VCS) used to track changes in files and coordinate work among multiple people. 
It allows developers to manage their projects effectively, ensuring collaboration and version history.
-->

<!-- Key Features -->
- **Distributed System**: 
  - Every user has a full copy of the project (repository), including the entire history.
  - No central dependency—work offline and sync when online.
- **Branching and Merging**:
  - Allows working on isolated features or fixes using branches.
  - Merging integrates branches into the main project.
- **Data Integrity**:
  - Uses SHA-1 hashing to ensure changes cannot be altered without detection.
  - Commit IDs (hashes) uniquely identify changes.
- **Efficient Performance**:
  - Local operations (e.g., commits, diffs, logs) are very fast since they do not depend on remote servers.
- **Free and Open Source**:
  - Git is open-source and available under the GNU General Public License (GPL).

---

## Git vs GitHub

<!-- 
Common confusion between Git and GitHub:

- **Git**: A version control tool to manage code locally and track changes.
- **GitHub**: A cloud-based platform for hosting and collaborating on Git repositories.
-->

- Git:
  - Installed locally on your system.
  - Handles operations like commits, branches, merges, and logs.
- GitHub:
  - Provides a remote repository for hosting your Git projects.
  - Offers additional features: pull requests, issues, CI/CD pipelines, etc.

---

## Why Learn Git?

<!-- 
Git is essential for:
- Managing code changes efficiently in software development.
- Collaborating with teams on shared projects.
- Maintaining a history of the project for rollback or review.
-->

- **Track Changes**:
  - Maintain a detailed log of all changes made to the project.
- **Collaboration**:
  - Work simultaneously with others without conflicts.
- **Backup**:
  - Keep your work secure and synchronized across multiple devices.
- **Mistake Recovery**:
  - Roll back to previous versions if bugs are introduced.

---

## How Git Works

<!-- 
Git's architecture revolves around four key areas:
1. Working Directory
2. Staging Area
3. Local Repository
4. Remote Repository
-->

- **Working Directory**:
  - The folder on your system where files are created and modified.
- **Staging Area**:
  - A middle layer where changes are prepared (staged) for a commit.
  - Allows selective tracking of changes.
- **Local Repository**:
  - The `.git` directory in your project.
  - Stores all commits and history locally.
- **Remote Repository**:
  - A version of the repository stored on a server like GitHub or GitLab.

---

## Git Workflow

<!-- 
Git workflow consists of:
1. Modifying files in the working directory.
2. Staging changes using `git add`.
3. Committing changes to the local repository with `git commit`.
4. Pushing to a remote repository using `git push`.
-->

- **Step 1**: Modify files in the working directory.

- **Step 2**: Add changes to the staging area:
  ```bash
  git add <file-name>
  ```

- **Step 3**: Save the changes in the local repository:
  ```bash
  git commit -m "Description of changes"
  ```

- **Step 4**: Push the changes to a remote repository:
  ```bash
  git push origin <branch-name>
  ```

---

## Frequently Asked Questions (FAQs)

<!-- 
FAQs to clarify common doubts about Git:
-->

1. **Can I use Git without GitHub?**
   - Yes, Git can be used locally for version control without GitHub.
   - GitHub is optional for hosting repositories remotely.

2. **What’s the difference between `git add` and `git commit`?**
   - `git add`: Moves changes to the staging area.
   - `git commit`: Saves staged changes into the repository history.

3. **Is Git only for coding projects?**
   - No, Git can track changes for any text-based project, including documentation, books, or research papers.
```