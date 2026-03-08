![My Git Logo](git-logo.png)
# 🚀 Git Lab 2
### Branching, Merging, Tags, and README Image

This lab demonstrates how to:

- Create a Git project and push it to GitHub
- Create and manage **branches**
- **Merge** branches
- **Delete** branches locally and remotely
- Switch branches **without committing changes**
- Create and manage **annotated tags**
- Add an **image to README**

---

# 1️⃣ Create Local Project and Push to Remote Repository

### Create project folder

```bash
mkdir Git_lab2
cd Git_lab2
```

### Initialize Git repository

```bash
git init
```

### Create README file

```bash
vi README.md
```

### Add files to staging

```bash
git add .
```

### Initial commit

```bash
git commit -m "initial commit"
```

### Rename branch to Main

```bash
git branch -m Main
```

### Connect repository to GitHub

```bash
git remote add orgin git@github.com:doniasobhyhelmy-gif/Git_lab2.git
```

### Push project to GitHub

```bash
git push -u orgin Main
```

---

# 2️⃣ Create Development Branch (dev)

### Create and switch to dev branch

```bash
git checkout -b dev
```

Output:

```
Switched to a new branch 'dev'
```

### Create dev file

```bash
touch dev_file.txt
```

### Add file

```bash
git add dev_file.txt
```

### Commit changes

```bash
git commit -m "adding dev file"
```

### Push dev branch

```bash
git push -u orgin dev
```

---

# 3️⃣ Create Testing Branch (test)

### Switch to Main branch

```bash
git checkout Main.
```

### Create test branch

```bash
git checkout -b test
```

### Create test file

```bash
touch test_file.txt
```

### Add file

```bash
git add test_file.txt
```

### Commit changes

```bash
git commit -m "adding test file"
```

### Push test branch

```bash
git push -u orgin test
```

---

# 4️⃣ Merge Branches into Main

### Merge dev branch

```bash
git merge dev
```

### Merge test branch

```bash
git merge test
```

### Push changes to Main

```bash
git push orgin Main
```

---

# 5️⃣ Delete Branches

## Delete branches locally

```bash
git branch -d dev
git branch -d test
```

## Delete branches remotely

```bash
git push orgin :dev
git push orgin --delete test
```

---

# 6️⃣ Checkout Another Branch Without Committing Changes

### Modify README

```bash
echo "this is half the work done " >>README.md
```

### Save uncommitted work

```bash
git stash
```

### Create emergency branch

```bash
git checkout -b emergency
```

### Return to Main

```bash
git checkout Main
```

### Restore changes

```bash
git stash pop
```

---

# 7️⃣ Create Annotated Tag

### Create tag

```bash
git tag -a v1.7 -m "release version 1.7"
```

### Push tag to remote repository

```bash
git push -u orgin Main v1.7
```

---

# 8️⃣ List Tags

```bash
git tag
```

Example output:

```
v1.7
```

---

# 9️⃣ Delete Tag Locally and Remotely

### Create another tag

```bash
git tag -a v1.8 -m "release version 1.8"
```

### Push tag

```bash
git push -u orgin Main v1.8
```

### Delete tag locally

```bash
git tag -d v1.8
```

### Delete tag remotely

```bash
git push orgin --delete v1.8
```

---

# 🔟 Add Image to README

### Check project files

```bash
ls
```

Example output:

```
dev_file.txt  git-logo.png  README.md  test_file.txt
```

### Add image to README

```bash
echo '![My Git Logo](git-logo.png)' >> README.md
```

### Stage files

```bash
git add README.md git-logo.png
```

### Commit changes

```bash
git commit -m "adding photo to README FILE"
```

### Push changes

```bash
git push -u orgin Main
```

---

# 🖼 README Image

![My Git Logo](git-logo.png)

