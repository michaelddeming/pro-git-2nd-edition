# 4.1 Git on the Server - The Protocols

- Intermediate Repository: A remote repository where collaborators can work on the same project, not matter the time or location. 

- Bare Repository: A Git repository that has no working directory. 

- The Protocols
    - 4 Main Protocols:
        1. Local: The remote repository is in another directory on the same host.
        - `$ git clone /srv/git/project.git`
        - `$ git clone file:///srv/git/project.git`
            - `file://`: Prefix repo filepath if you want a clean copy of the repository with extraneous references or objects left out 
        2. HTTP:
            -  Smart HTTP: A single URL link that is synced to a remote repository, where users can push and pull from said link.
            - Dump HTTP: 
        3. Secure Shell (SSH):
            - `$ git clone ssh://[user@]server/project.git` or `$ git clone [user@]server:project.git`
        
        4. Git

# 4.2 Git on the Server - Getting Git on a Server

# 4.3 Git on the Server - Generating Your SSH Public Key

- User SSH Keys are found within the `~/.ssh` directory. 
    - Check for current SSH keys first by using `cd` and `ls` in your CLI. 
    - `id_###`, *private key*, and a matching `.pub` file, *public key*.
        - If these files are not found, run `ssh-keygen`.

# 4.4 Git on the Server - Setting Up the Server

# 4.5 Git on the Server - Git Daemon

- Git Daemon: 

# 4.6 Git on the Server - Smart HTTP

- CGI:

- `git-http-backend`:

# 4.7 Git on the Server - GitWeb

- GitWeb: Simple web-based visualizer that comes with Git.

# 4.8 Git on the Server - GitLab

- GitLab:

- Blocking Users: Prevents the user from logging into the GitLab instance, but all the data under the user's namespace is preserved. 

- Destroying Users: Completely removes them from the database and filesystem, all data in namespace is removed. 

# 4.9 Git on the Server - Third Party Hosted Options

- Hosting Options: https://archive.kernel.org/oldwiki/git.wiki.kernel.org/index.php/GitHosting.html

