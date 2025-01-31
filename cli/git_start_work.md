# Start Work Day

Before starting your work, ensure you have the latest updates from `main` or applicable `dev` branch and apply them to your working branch.

### **1. Switch to `main` and Pull the latest changes**
```bash
git checkout main
```
```bash
git pull origin main
```
This ensures your `main` branch is up-to-date with the remote repository.


### **2. Switch back to your feature branch**
```bash
git checkout <your-branch-name>
```
This returns you to the branch where you were working.


### **3. Merge the latest `main` updates into your branch**
```bash
git merge main
```
This brings the latest changes from `main` into your branch to keep it in sync.


### **4. Verify everything is Up-to-Date**
```bash
git status
```
Ensure there are no unexpected conflicts or uncommitted changes before you start coding.

Now, you're ready to start working with the latest updates! 🚀
