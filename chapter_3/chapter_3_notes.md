
# 3.1 Git Branching - Branches in a Nutshell

- Branching: Diverge from the main line of development and continue to do wokr without messing with that main line. 
    - Default name in Git is `master`. 

- Blobs: Files that have been checksummed and hashed and stored in the Git repository.

- Creating Branches:
    - `HEAD` is a pointer to the current *working branch*, creating a new branch does not move the `HEAD` pointer, must move manually. 
        - `git log --decorate`: Show the `HEAD` pointer location.
    - `git branch <newbranchname>`: Create a new branch from the current working branch. 
    - `git checkout <branchname>`: Switch the `HEAD` pointer to the indicated branch. 
    - `git checkout -b <newbranchname>`: Create a new branch and auto switch the `HEAD` pointer to it. 
    - `git switch`: Can be used instead of `git checkout`.
    - `git switch testing-branch`: Switch to an exisiting branch.
    - `git switch -c new-branch`: Create a new branch and switch the `HEAD` pointer to it. The flag `-c` stands for "create", can also use `--create`.
    - `git switch -`: Return to your previously checkout out branch.

# 3.2 Git Branching - Basic Branching and Merging

- Fast-forward: 

- `git branch -d <branchname>`: `-d` flag indicates a deletion of the given branch. 

# 3.3 Git Branching - Branch Management

- Branch Management:
    - `git branch`: By itself, when called, will show all branches.
    - `git branch -v`: Shows the last commit on each branch.
    - `git branch --merged`: Shows which branches are already merged into the branch you're on. 
    - `git branch --no-merged`: Shows all branches that contain work you haven't merged in. 

# 3.4 Git Branching - Branching Workflows

- Topic Branch: A short-lived branch that you create and use for a single particular feature or related work. 

# 3.5 Git Branching - Remote Branches

- `git ls-remote <remote>` or `git remote show <remote>`: Get a full list of remote references.

- Remote-tracking Branches: 

# 3.6 Git Branching - Rebasing

- Rebasing

# 3.7 Git Branching - Summary

