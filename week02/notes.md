1) What did pwd print?

Ans. pwd printed /Users/devarthtandan, i.e. it printed the present working directory (showing the user where they are currently).

2) What did 'ls -a' show that plain 'ls' did not?

Ans. 'ls -a' shows the system’s hidden files (dot files) as well, which plain 'ls' does not. 

3) Pick one line from 'ls -l'. What do you think the first column means? 

Ans. drwx------+  13 devarthtandan  staff    416 23 Aug 19:20 Desktop
The first column denotes only the file type and the access level of the file. 

4) Why does that work from where you are standing? Which kind of path is coding-cafe/week02? Absolute or relative?

Ans. It works because there is a folder named coding-cafe in our location, which further has a folder called week 02 which is why it opens. It is a relative path, because if there was another location with the same file names it would have worked over there as well. 

5) mv did two different jobs. What were they?

Ans. mv moved the file in the first instance, and renamed the file in the second instance. 

6) How many folders are on your PATH? (They are separated by :)

Ans. 10

7) Write down exactly where your python3 lives. You will need this again in a minute.

Ans. /usr/bin/python3

8) Compare your answer to 7 with the person next to you. Are they the same? If not, why might that be?

Ans. The answer was the same. 

9) What exactly did the shell say? Explain the error in your own words, using the word PATH.

Ans. zsh: command not found: pyton3
Due to the input of an invalid command, the shell showed a 'command not found' error. The command pyton3 does not exist on the path, so the shell could not locate it. 

10) .venv did not appear with plain ls. Why not? 

Ans. Because it is a hidden/dot file, and is visible only with lsn -a not ls. 

11) What changed about your prompt?

Ans. The prompt starts with (.venv) at the very beginning now. 

12) Compare this with what you wrote down for question 7. Is it the same path? If not, what does that tell you about what activate actually did to your PATH?

Ans. /Users/devarthtandan/coding-cafe/.venv/bin/python3. 
It is not the same path. It created a smaller, self sufficient box within the file system which changes the path. 

13) What is in the second list that was not in the first?

Ans. The first list showed the packages in the virtual environment. However, after  installation of other packages in the virtual environment, more packages were visible in the second list. 

14) Where does python3 point now?

Ans. It points back to the global executable file (which we began with initially), it basically takes us outside .venv.

15) Find what ls -h does. Write it in your own words.

Ans. 'ls -h' simply makes the file size more readable, which is easier to understand for us. 

16) What is the difference between what Ctrl + C and Ctrl + D did?

Ans. Ctrl + C basically ends the currently running process byu sending an interrupt signal, whereas Ctrl + D signals the end of input to exit a shell. 