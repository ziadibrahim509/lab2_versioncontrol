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

2️⃣ Create Branches & Add Files

Dev branch

git checkout -b dev
echo "dev file" > dev.txt
git add dev.txt
git commit -m "Add dev file"
git push origin dev

Test branch

git checkout main
git checkout -b test
echo "test file" > test.txt
git add test.txt
git commit -m "Add test file"
git push origin test

3️⃣ Merge Branches into Main
git checkout main
git merge dev
git merge test
git push origin main

4️⃣ Tags

Create an annotated tag:

git tag -a v1.7 -m "Version 1.7 release"
git push origin v1.7

List tags:

git tag

Delete tags:

git tag -d v1.7               # locally
git push origin --delete tag v1.7  # remotely






