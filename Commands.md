### Basic Commands
1. **`git init`**  
   Initializes a new Git repository in the current directory.  

2. **`git clone <repository-url>`**  
   Clones an existing remote repository to your local machine.  

3. **`git status`**  
   Displays the current status of the working directory and staging area.  

4. **`git add <file>`**  
   Stages changes in a specified file for the next commit.  

5. **`git add .`**  
   Stages all changes in the current directory for the next commit.  

6. **`git commit -m "<message>"`**  
   Saves staged changes to the repository with a message describing the changes.  

7. **`git push origin <branch>`**  
   Uploads local branch commits to the corresponding remote branch.  

8. **`git pull origin <branch>`**  
   Fetches and merges changes from the remote repository into the current branch.  

### Branching and Merging  
9. **`git branch`**  
   Lists all branches in the repository, marking the current branch with an asterisk.  

10. **`git branch <branch-name>`**  
    Creates a new branch with the specified name.  

11. **`git checkout <branch>`**  
    Switches to the specified branch.  

12. **`git switch <branch-name>`**  
    Switches to the specified branch (modern alternative to `checkout`).  

13. **`git checkout -b <branch-name>`**  
    Creates and switches to a new branch in a single step.  

14. **`git merge <branch-name>`**  
    Merges changes from the specified branch into the current branch.  

15. **`git branch -d <branch-name>`**  
    Deletes the specified branch if it has been fully merged.  

### Viewing Changes  
16. **`git log`**  
    Displays a history of commits, including commit IDs, authors, and messages.  

17. **`git log --oneline`**  
    Shows a condensed, one-line view of commit history.  

18. **`git diff`**  
    Displays differences between the working directory and the repository.  

19. **`git diff <branch1> <branch2>`**  
    Compares the differences between two branches.  

### Undoing Changes  
20. **`git reset <file>`**  
    Unstages the specified file from the staging area.  

21. **`git reset --hard <commit-hash>`**  
    Resets the repository to the specified commit, discarding all changes.  

22. **`git revert <commit-hash>`**  
    Creates a new commit that undoes the changes from a specific commit.  

### Stashing  
23. **`git stash`**  
    Temporarily stores uncommitted changes for later use.  

24. **`git stash list`**  
    Displays a list of all stashes.  

25. **`git stash apply`**  
    Re-applies the most recent stash without deleting it from the stash list.  

26. **`git stash drop`**  
    Deletes the most recent stash from the list.  

### Tags and Releases  
27. **`git tag <tag-name>`**  
    Creates a new tag for marking specific commits (e.g., release versions).  

28. **`git tag -a <tag-name> -m "<message>"`**  
    Creates an annotated tag with a message.  

29. **`git show <tag-name>`**  
    Displays information about the specified tag, including the commit it points to.  

### Remote Commands  
30. **`git remote -v`**  
    Lists all remote repositories and their URLs.  