# Best Practices:
- "git pull && git push": This is like regularly saving your work. You do this before you start working and when you finish for the day. It helps avoid mixing up changes made by you and others.
- Merge Main Branch: Think of it like updating your work with the latest changes from others. You do this once a day to stay updated.
- Small Changes Often: It's like breaking big tasks into smaller ones. It's easier to manage and fix problems this way.
- Don't Erase History: Imagine if you could see all the changes made to a document. "Force push" and "rebase" are like erasing parts of that history. It's not good for teamwork and wastes time.
- Feature Flagging: It's like hiding some parts of your code until it's ready. This helps with testing and making sure everything works before showing it to everyone.

# Code Best Practices:
- Python Code: Always test your code and write it in a clean, clear way. Python is picky about syntax, so testing is super important.
- Canonical Python Code: This means writing code in a way that's easy to understand and follow. Use shortcuts when they make sense.
- Async Programming: It's like doing multiple things at once. This makes your code faster by not waiting around for one thing to finish before moving on to the next.
- Avoid Threading: Threading is like trying to do multiple things at once in Python, but it's not very efficient. It's better to use other methods if you need to do this.


# Login / Servers

login:
```bash
gcloud auth application-default login
```
server:
```bash
uvicorn app.main:app
```

# Git

## Set current branch to the state of origin/main

Fetch the latest changes from the remote repository to ensure you have the most recent state:
```bash
git fetch origin
```

Reset your current branch <my-branch> to <origin/main>:
```bash
git reset --hard origin/main
```
Switch branches:
```
git checkout <branch-name>
```

Create and switch to a new branch
```
git checkout -b <new-branch-name>
```
### Commit Your Changes to a Different Branch
Stash Your Changes
Stash both staged and unstaged changes:
```
git stash
```
### Apply Your Stashed Changes
Switch to the correct branch:
```
git checkout <your-target-branch>
```
Apply the stashed changes:
```
git stash apply
```

### Add and Commit Your Changes
Add your changes:
```
git add .
```
Commit your changes:
```bash
git commit -m "Your commit message"
```

### Push Your Changes
Push your changes to the remote repository:
```
git push origin <your-target-branch>
```

## Git Merge Strategies
Recursive
Merge two branches using the recursive strategy:
```bash
git merge -s recursive <branch1> <branch2>
```
Resolve
Merge two branches using the resolve strategy:
```bash
git merge -s resolve <branch1> <branch2>
```

Octopus
Merge multiple branches using the octopus strategy:

```bash
git merge -s octopus <branch1> <branch2> <branch3> ... <branchN>
```

Ours
Merge multiple branches using the ours strategy:
```bash
git merge -s ours <branch1> <branch2> <branchN>
```
Subtree
Merge subtree branches using the subtree strategy:

```bash
git merge -s subtree <branchA> <branchB>
```


## IntelliJ
inline:
```mathematica
Ctrl + Alt + N
```


## useful
- https://www.uvicorn.org/deployment/
- https://docs.python.org/3/howto/logging.html
- https://docs.python.org/3/library/urllib.parse.html
- https://docs.python.org/3/whatsnew/3.12.html#asyncio
- https://docs.python.org/3/whatsnew/3.12.ht
