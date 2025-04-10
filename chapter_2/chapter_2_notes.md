
# 2.1 Git Basics - Getting a Git Repository

- Two Ways to Typically Get a Git Repository
    1. Turn a local directory, that is not currently a Git repo. and turn it into a Git repo. 
        - `cd` in the project directory. 
        - type command `git init`
    2. `clone` an exisiting Git repo. from elsewhere.
        - `git clone`
        - `git clone <url>`

# 2.2 Git Basics - Recording Changes to the Repository

- Files in the working directory change be in 2 states:
    1. `tracked`: Files that were in the last snapshot, as well as any newly staged files; they can be unmodified, modified, or staged. 
    2. `untracked`: Files that were not included in the last snapshot and are not in the staging area. 

- Checking Status of Files: 
    - `git status`
    - `git status -s` or `git status --short` (short status)

- NOTE: `main`(in GitHub) vs `master`(in Git) for default branch.

- Tracking a File: `git add`
    - `git add filename`
    - `git add directory`

- Ignoring Files: `.gitignore`
    - Specify *patterns* for files and file types to be ignored by Git.
    - Rules For Patterns:
        1. Blanks lines or lines starting with `#` are ignored.
        2. Standard glob patterns work, and will be applied recursively throughout the entire working tree.
            - Glob Patterns: 
        3. You can start patterns with a forward slash `/` to avoid recursivity.
        4. You can end patterns with a forward slash `/` to specify a directory.
        5. You can negate a pattern by starting it with an exclamation point `!`.

![alt text](image.png)

- View Staged Changes 
    - `git diff`: Compares what is in your working directory with what is in your staging area.
    - `git diff --staged` or `git diff --cached`: See what you have staged that will go into your next commit. 
    - `git difftool`: View file differences with external tools not Git standard. 

- Commiting Your Changes
    - `git commit`: Commits staged files to the main branch. 
    - `git commit -v`: Provides an explicit reminder of what you've modified. 
    - `git commit -m *"message"*`: Bypass the text editor for providing a message to the commit, and allow for an in-line message to be provided at the time of call. 
