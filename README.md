\# Git Mastery Task



A small project demonstrating the Git and GitHub command-line workflow.



\## What this repo contains



\- `my\_project\_file.txt`: a simple text file

\- `.gitignore`: tells Git to ignore `\*.log` files

\- `README.md`: this documentation



\## Prerequisites



\- Git installed (`git --version`)

\- A GitHub account

\- GitHub CLI (`gh`) installed and logged in (`gh auth login`)



\## Steps performed



1\. Initialized a local repo with `git init`

2\. Created a text file and a `debug.log` file

3\. Added `\*.log` to `.gitignore` so `debug.log` is not tracked

4\. Staged and committed the files

5\. Created a public repo and pushed from the command line



\## Commands used



```bash

mkdir git-mastery-task

cd git-mastery-task

git init

echo "This is my first command-line push to GitHub!" > my\_project\_file.txt

echo "Error: Something went wrong" > debug.log

echo "\*.log" > .gitignore

git status

git add .

git commit -m "Initial commit: Added text file, .gitignore and README"

git branch -M main

gh repo create git-mastery-task --public --source=. --remote=origin --push

```



\## Verifying .gitignore works



Run `git status`. The file `debug.log` should not appear in the list, which confirms it is being ignored.



\## Author



Vaishnavi

