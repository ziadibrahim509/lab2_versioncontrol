Got it! Here’s the **entire README content in one single Markdown block**, fully ready to copy-paste into GitHub:

```markdown
# 📝 Lab 2: Version Control Project

![GitHub repo size](https://img.shields.io/github/repo-size/ziadibrahim509/lab2_versioncontrol) 
![GitHub last commit](https://img.shields.io/github/last-commit/ziadibrahim509/lab2_versioncontrol) 

---

## 🌟 Overview
This project demonstrates the use of **Git** and **GitHub** for version control.  
It covers:

- Creating and managing **branches** (`dev` & `test`)  
- Merging changes into **main**  
- Using **annotated tags**  
- Adding **images** and updating `README.md`  

---

## 🗂 Project Structure

```

project_git/
│
├── README.md        # Project documentation
├── dev.txt          # Created in 'dev' branch
├── test.txt         # Created in 'test' branch
├── image.png        # Image added to README

````

---

## 🔧 Git Workflow

### 1️⃣ Initialize Project

```bash
git init
git add README.md
git commit -m "Initial commit"
git branch -M main
git remote add origin <repo-url>
git push -u origin main
````

---

### 2️⃣ Create Branches & Add Files

**Dev branch**

```bash
git checkout -b dev
echo "dev file" > dev.txt
git add dev.txt
git commit -m "Add dev file"
git push origin dev
```

**Test branch**

```bash
git checkout main
git checkout -b test
echo "test file" > test.txt
git add test.txt
git commit -m "Add test file"
git push origin test
```

---

### 3️⃣ Merge Branches into Main

```bash
git checkout main
git merge dev
git merge test
git push origin main
```

---

### 4️⃣ Tags

* Create an **annotated tag**:

```bash
git tag -a v1.7 -m "Version 1.7 release"
git push origin v1.7
```

* List tags:

```bash
git tag
```

* Delete tags:

```bash
git tag -d v1.7               # locally
git push origin --delete tag v1.7  # remotely
```

---

### 5️⃣ Adding Images

![Project Image](image.png)

**To add an image to README.md**:

```markdown
![Alt text](image.png)
```

* Upload the image to the repo → commit changes.

---

## 🔄 Working with Branches

* **Checkout another branch without committing changes**:

```bash
git stash
git checkout branch_name
git stash pop
```

* **Remove branches**:

```bash
git branch -d dev              # locally
git push origin --delete dev   # remotely
```

---

## ✅ Summary

This project demonstrates:

* Proper **branching and merging** workflow
* **Tagging versions** of the project
* **Staging, committing, and pushing** changes
* Managing files and **images on GitHub**

---

### 💡 Tip

Use this README as a **guide for labs or portfolio projects** — it’s clean, professional, and fully GitHub-compatible.

```

---

If you want, I can make a **next-level version** with a **clickable Table of Contents, colors, and extra emojis**, so it looks like a **portfolio-ready GitHub project**.  

Do you want me to do that?
```
