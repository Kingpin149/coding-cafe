# Lab 4 Notes
## Question 1
--global here applied the configuration across all the repositories in the whole user environment rather than just a single/local project or function. If I left it out, it would default to --local and will be accessible within the current repository only. 
## Question 2
hidden directories .git and .venv appeared in ls -a but not in ls. .git is git's database for the repository. .venv is the python virtual runtime environment.
## Question 3
roughly hundreds to thousands of files. yes, the .venv/ file. it contains hundreds to thousands files which i cannot understand primarily because i didnt write them
## Question 4
.venv/ and the thousands of files within it disappeared from git status. compiled python files which i mentioned under git ignore (such as __pycache__/ or *.pyc) or other files like .DS_Store also disappeared. instead of these files, only .gitignore and other project files are visible.
## Question 5
.gitignore should be committed. this ensures that anyone else who works on the repository automatically shares the same ignore rules. 
## Question 6
README.md moved from "Untracked files:" to "Changes to be committed:". In the three places model, it moved fromt he Working Directory to the Staging Area, and it is prepared to be permanently recorded into the repository on the next commit. 
## Question 7
After the command, git printed:
[main (root-commit) 39496fc] Lab work so far
 6 files changed, 86 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 README.md
 create mode 100644 lab4.md
 create mode 100644 lab4.nd
 create mode 100644 week02/lab01-log.txt
 create mode 100644 week02/notes.md
It says that 6 files changed
## Question 8
39496fc. They serve as the unique identifier for this particular commit snapshot
## Question 9
1. Create/edit file in the working directory (writing lab4/notes.md)
2. Check status (using git status)
3. Moving files into the staging area using git add
4. Committing the file into the repository history using git commit
## Question 10
README.md is given a prominent place in the root directory because it follows a universal open-source convention designed to immediately catch a reader's attention as the primary entry point to a project. Unlike internal files like lab4/notes.md that cover isolated assignments, the root README.md provides high-level context for the entire repository—explaining what the project is, who made it, and how it is organized—and platforms like GitHub automatically render it as the project's public homepage and landing guide.
## Question 11
When you run gh auth login, it connects to your GitHub account and saves a secure authentication token directly to your computer. At the same time, it tells Git to use GitHub CLI as its credential manager. That way, whenever you push changes, Git just grabs that stored token in the background to confirm it's really you—so you never have to stop and re-type your password.
## Question 12
On the GitHub front page, you see the rendered contents of your README.md file. GitHub does this by default because it's built to treat a root README as the project's natural front porch—it automatically grabs the file and displays it so anyone landing on the repo can immediately read what it is, who made it, and what's inside without having to click around.
## Question 13
No, pushing didn't change your local commit history at all. All your commit hashes, messages, and timestamps are exactly the same; the only thing that shifted is Git updating the remote tracking pointer (origin/main) to sit right alongside your local main, confirming your machine and GitHub are finally in sync.
## Question 14
If a repository doesn't exist on GitHub at all, it simply lives only on your local machine—meaning there is no cloud backup, no remote synchronization, and zero way to collaborate over GitHub. A private repository, on the other hand, exists fully on GitHub's servers, benefits from remote backups, and lets you selectively grant access to specific people (like your TAs) through invitations, even though GitHub hides it completely behind a 404 screen to keep it invisible from the general public.