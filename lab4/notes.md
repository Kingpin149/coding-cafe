# Lab 4 Notes
## Question 1
- --global here applied the configuration across all the repositories in the whole user environment rather than just a single/local project or function. If I left it out, it would default to --local and will be accessible within the current repository only. 
## Question 2
hidden directories .git and .venv appeared in ls -a but not in ls. .git is git's database for the repository. .venv is the python virtual runtime environment.
## Question 3
-roughly hundreds to thousands of files. yes, the .venv/ file. it contains hundreds to thousands files which i cannot understand primarily because i didnt write them
## Question 4
- .venv/ and the thousands of files within it disappeared from git status. compiled python files which i mentioned under git ignore (such as __pycache__/ or *.pyc) or other files like .DS_Store also disappeared. instead of these files, only .gitignore and other project files are visible.
## Question 5
- .gitignore should be committed. this ensures that anyone else who works on the repository automatically shares the same ignore rules. 
## Question 6
- README.md moved from "Untracked files:" to "Changes to be committed:". In the three places model, it moved fromt he Working Directory to the Staging Area, and it is prepared to be permanently recorded into the repository on the next commit. 
## Question 7
- After the command, git printed:
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
- 39496fc. They serve as the unique identifier for this particular commit snapshot
