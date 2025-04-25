# Git Branch Deletion Practice 🚀

This repository is created to practice how to delete Git branches both locally and remotely. It is part of learning the **Git Fundamentals**.

---

## 🧠 What You'll Learn

- How to safely delete local branches.
- Understand the difference between the `-d` and `-D` flags.
- How to delete remote branches using `git push origin --delete`.

---

## 📘 Local Branch Deletion

### ✅ Safe Deletion (Only Merged Branches)
To safely delete a branch that has already been merged:
```bash
git branch -d your-branch-name
```

### ❗ Force Deletion (Even If Not Merged)
To delete a branch forcefully, even if it has unmerged changes:
```bash
git branch -D your-branch-name
```

---

## 🌐 Remote Branch Deletion

### 🔄 Deleting a Remote Branch
To remove a branch from the remote repository (e.g., GitHub):
```bash
git push origin --delete your-branch-name
```

---

## 🧪 Practice Setup

### Step 1: Create a Test Branch
Create a new branch for testing:
```bash
git checkout -b test-feature
```

### Step 2: Delete It Locally
Delete the test branch locally:
```bash
git branch -d test-feature
```

### Step 3: Push and Delete Remotely
Push the branch to the remote repository and then delete it:
```bash
git push origin test-feature
git push origin --delete test-feature
```

---

## 📁 Example Use Case

A practical example to simulate creating, merging, and deleting a branch:

1. Create a feature branch:
    ```bash
    git checkout -b feature-x
    ```

2. Make changes and commit:
    ```bash
    # Make changes in your files
    git commit -am "Feature X done"
    ```

3. Merge the branch into the main branch:
    ```bash
    git checkout main
    git merge feature-x
    ```

4. Delete the branch locally:
    ```bash
    git branch -d feature-x
    ```

5. Delete the branch remotely:
    ```bash
    git push origin --delete feature-x
    ```

---
