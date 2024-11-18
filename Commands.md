
---

### Basic Commands  

1. **Initialize a new Git repository**  
   Initializes a new Git repository in the current directory.  
   ```bash
   git init
   ```

2. **Clone an existing repository**  
   Clones an existing remote repository to your local machine.  
   ```bash
   git clone <repository-url>
   ```

3. **Check the status of your working directory**  
   Displays the current status of the working directory and staging area.  
   ```bash
   git status
   ```

4. **Stage specific changes for the next commit**  
   Stages changes in a specified file for the next commit.  
   ```bash
   git add <file>
   ```

5. **Stage all changes for the next commit**  
   Stages all changes in the current directory.  
   ```bash
   git add .
   ```

6. **Commit staged changes**  
   Saves staged changes to the repository with a descriptive message.  
   ```bash
   git commit -m "<message>"
   ```

7. **Push local changes to the remote branch**  
   Uploads commits from the local branch to the corresponding remote branch.  
   ```bash
   git push origin <branch>
   ```

8. **Pull and merge remote changes**  
   Fetches and merges changes from the remote repository into the current branch.  
   ```bash
   git pull origin <branch>
   ```

---

### Branching and Merging  

9. **List all branches**  
   Lists all branches in the repository, marking the current branch with an asterisk.  
   ```bash
   git branch
   ```

10. **Create a new branch**  
    Creates a new branch with the specified name.  
    ```bash
    git branch <branch-name>
    ```

11. **Switch to another branch**  
    Switches to the specified branch.  
    ```bash
    git checkout <branch>
    ```

12. **Switch to another branch (modern command)**  
    A modern alternative to `checkout` for switching branches.  
    ```bash
    git switch <branch-name>
    ```

13. **Create and switch to a new branch**  
    Creates and switches to a new branch in one step.  
    ```bash
    git checkout -b <branch-name>
    ```

14. **Merge another branch into the current branch**  
    Merges changes from the specified branch into the current branch.  
    ```bash
    git merge <branch-name>
    ```

15. **Delete a branch**  
    Deletes the specified branch if it has been fully merged.  
    ```bash
    git branch -d <branch-name>
    ```

---

### Viewing Changes  

16. **View the commit history**  
    Displays a history of commits, including commit IDs, authors, and messages.  
    ```bash
    git log
    ```

17. **View a condensed commit history**  
    Shows a one-line view of commit history.  
    ```bash
    git log --oneline
    ```

18. **See changes in the working directory**  
    Displays differences between the working directory and the repository.  
    ```bash
    git diff
    ```

19. **Compare two branches**  
    Displays the differences between two branches.  
    ```bash
    git diff <branch1> <branch2>
    ```

---

### Undoing Changes  

20. **Unstage a file**  
    Removes the specified file from the staging area.  
    ```bash
    git reset <file>
    ```

21. **Hard reset to a specific commit**  
    Resets the repository to the specified commit, discarding all changes.  
    ```bash
    git reset --hard <commit-hash>
    ```

22. **Revert a specific commit**  
    Creates a new commit that undoes the changes from a specific commit.  
    ```bash
    git revert <commit-hash>
    ```

23. **Remove untracked files**  
    Deletes all untracked files in the working directory.  
    ```bash
    git clean -f
    ```

---

### Stashing  

24. **Stash changes temporarily**  
    Temporarily stores uncommitted changes for later use.  
    ```bash
    git stash
    ```

25. **List all stashes**  
    Displays a list of all stashes.  
    ```bash
    git stash list
    ```

26. **Re-apply the latest stash**  
    Applies the most recent stash without removing it from the stash list.  
    ```bash
    git stash apply
    ```

27. **Delete the most recent stash**  
    Deletes the most recent stash from the stash list.  
    ```bash
    git stash drop
    ```

28. **Apply and drop the stash simultaneously**  
    Applies and removes the latest stash.  
    ```bash
    git stash pop
    ```

---

### Tags and Releases  

29. **Create a lightweight tag**  
    Marks a specific commit with a simple tag.  
    ```bash
    git tag <tag-name>
    ```

30. **Create an annotated tag**  
    Creates a tag with additional information like a message.  
    ```bash
    git tag -a <tag-name> -m "<message>"
    ```

31. **Show tag details**  
    Displays information about a specific tag and its associated commit.  
    ```bash
    git show <tag-name>
    ```

32. **Push tags to the remote repository**  
    Uploads all local tags to the remote repository.  
    ```bash
    git push --tags
    ```

---

### Advanced Commands  

33. **Cherry-pick a commit**  
    Applies a specific commit from another branch to the current branch.  
    ```bash
    git cherry-pick <commit-hash>
    ```

34. **Amend the last commit**  
    Modify the most recent commit (e.g., to correct the commit message).  
    ```bash
    git commit --amend
    ```

35. **Rebase a branch**  
    Moves or combines commits from one branch onto another.  
    ```bash
    git rebase <branch>
    ```

36. **Interactive rebase**  
    Allows you to edit, reorder, or squash commits during a rebase.  
    ```bash
    git rebase -i <base-branch>
    ```

37. **Show a specific commit**  
    Displays detailed information about a specific commit.  
    ```bash
    git show <commit-hash>
    ```

38. **Bisect to find a bug**  
    Finds the commit that introduced a bug using a binary search.  
    ```bash
    git bisect
    ```

39. **Squash commits**  
    Combine multiple commits into one during a rebase.  
    ```bash
    git rebase -i
    ```

40. **Blame a file**  
    Displays the author and commit details for each line of a file.  
    ```bash
    git blame <file>
    ```

41. **Restore changes**  
    Restores working directory files to a previous state.  
    ```bash
    git restore <file>
    ```

42. **Track file renames**  
    Identifies when files have been renamed between commits.  
    ```bash
    git log --follow <file>
    ```

43. **Set a remote URL**  
    Updates the URL of an existing remote repository.  
    ```bash
    git remote set-url origin <new-url>
    ```

44. **Remove a remote**  
    Deletes a remote repository from your local configuration.  
    ```bash
    git remote remove <remote-name>
    ```

45. **Show all changes for a file**  
    Displays the complete history of changes to a specific file.  
    ```bash
    git log -- <file>
    ```

46. **View staged changes**  
    Shows differences between the staging area and the last commit.  
    ```bash
    git diff --cached
    ```

47. **Remove a file from Git but keep it locally**  
    Removes a file from the repository while retaining it locally.  
    ```bash
    git rm --cached <file>
    ```

48. **Tag a commit after pushing**  
    Tags a specific commit even if it's not the latest one.  
    ```bash
    git tag -a <tag-name> <commit-hash> -m "<message>"
    ```

49. **List unpushed commits**  
    Shows commits that haven't been pushed to the remote branch.  
    ```bash
    git log origin/<branch>..<branch>
    ```

50. **Check the Git version**  
    Displays the installed version of Git.  
    ```bash
    git --version
    ```