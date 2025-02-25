# Step 1: Install and Configure Git

### ✅ Check if Git is Installed
```bash
git --version
```
If Git is not installed, download it from [git-scm.com](https://git-scm.com/).

### ✅ Configure Git Username and Email
```bash
git config --global user.name "asrafi436"
git config --global user.email "asrafi436@gmail.com"
```

### ✅ Verify Git Configuration
```bash
git config --global --list
```

---

# Step 2: Work with a Git Repository

### ✅ Create a New Folder and Initialize Git
```bash
mkdir git-demo
cd git-demo
git init
```

### ✅ Create a README.md File
```bash
echo "# Git Demo Project" > README.md
```

### ✅ Check Git Status
```bash
git status
```

### ✅ Stage and Commit the README.md File
```bash
git add README.md
git commit -m "Initial commit with README.md"
```

### ✅ Create a New GitHub Repository
1. Go to [GitHub](https://github.com) and create a new repository named **git-demo**.
2. Copy the **HTTPS URL** of the repository (e.g., `https://github.com/asrafi436/git-demo.git`).

### ✅ Add Remote Repository and Push
```bash
git remote add origin https://github.com/asrafi436/git-demo.git
git remote -v

git branch -M main
git push -u origin main
```
If prompted, enter your GitHub username and password (or personal access token if using 2FA).

✅ You should now see your `README.md` file on GitHub.

---

# Step 3: Branching and Merging

### ✅ Create and Switch to a New Branch
```bash
git checkout -b feature-branch
git branch
```

### ✅ Modify README.md
Add more details to the project:
```bash
echo "This project demonstrates Git workflows including branching and merging." >> README.md
```

### ✅ Stage and Commit Changes
```bash
git add README.md
git commit -m "Updated README.md with more project details"
```

### ✅ Push the Feature Branch to GitHub
```bash
git push -u origin feature-branch
```

### ✅ Merge Feature Branch into Main
1. Switch back to `main`:
```bash
git checkout main
```

2. Merge the `feature-branch` into `main`:
```bash
git merge feature-branch
```

3. Push the updated `main` branch to GitHub:
```bash
git push origin main
```

### ✅ Clean Up (Optional)
Delete the `feature-branch` locally if no longer needed:
```bash
git branch -d feature-branch
```

---

# Final Check
1. Go to your GitHub repository: [https://github.com/asrafi436/git-demo](https://github.com/asrafi436/git-demo).
2. Confirm:
   - The updated `README.md` is visible.
   - Both `main` and `feature-branch` exist under **Branches**.

