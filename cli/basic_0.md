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
