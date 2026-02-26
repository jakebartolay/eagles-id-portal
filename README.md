<p align="center">
  <a href="https://laravel.com" target="_blank">
    <img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo">
  </a>
</p>

<p align="center">
  <a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
  <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
  <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
  <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Installing Laravel Project

Follow these steps to set up the project locally:

---

### Step 1: Download Required Tools
Install the following tools:

- **Visual Studio Code**: [https://code.visualstudio.com/](https://code.visualstudio.com/)  
- **XAMPP** (Local PHP Server + MySQL): [https://www.apachefriends.org/](https://www.apachefriends.org/)  
- **Composer** (PHP dependency manager): [https://getcomposer.org/download/](https://getcomposer.org/download/)  
- **Git** (Version Control): [https://git-scm.com/downloads](https://git-scm.com/downloads)  

---

### Step 2: Clone the Project
1. Right-click on your desktop → select **Git Bash Here**  
2. Type the command to clone the project:

```bash
git clone https://github.com/jakebartolay/eagles-id-portal.git
cd eagles-id-portal

### Step 3: Change .env.example to .env
- Copy .env.example → rename to .env
- .env contains your local environment settings like database credentials.

### Step 4: Install Composer
composer install
php artisan key:generate

### Step 5: run the laravel project in Vs code terminal
php artisan serve

### GITHUB PUSH AND PULL BRACHES 

=============================
OJT GIT CHEAT SHEET - STEP BY STEP
=============================

1️⃣ START FROM MAIN BRANCH
Always make sure main branch is up-to-date:

git checkout main
git pull origin main

---

2️⃣ CREATE A FEATURE BRANCH
Decide your task:
- Frontend work → feature/frontend
- Backend work → feature/backend

# Frontend branch
git checkout -b feature/frontend

# Backend branch
git checkout -b feature/backend

# Check current branch
git branch

---

3️⃣ STASH CHANGES (Optional)
If you have uncommitted work and need to switch branches:

git stash                 # save changes temporarily
git checkout feature/frontend  # switch branch
git stash apply           # restore your changes

---

4️⃣ PULL LATEST CHANGES
Always pull the latest branch updates:

git pull origin feature/frontend  # or feature/backend

---

5️⃣ DO YOUR WORK
- Add your changes to the branch:

git add .
git commit -m "Brief description of your changes"

---

6️⃣ PUSH CHANGES TO GITHUB

git push origin feature/frontend  # or feature/backend

---

7️⃣ MERGE FEATURE BRANCHES
If backend changes affect frontend, merge backend into frontend:

git checkout feature/frontend
git merge feature/backend
git add .          # if conflicts resolved
git commit -m "Merge backend changes into frontend"
git push origin feature/frontend

---

8️⃣ USE TESTING BRANCH (Recommended)
Combine frontend + backend changes to test before main:

# Create testing branch from main
git checkout main
git checkout -b testing
git push origin testing

# Merge features into testing
git checkout testing
git merge feature/frontend
git merge feature/backend

# Test everything locally
php artisan serve

---

9️⃣ MERGE INTO MAIN
Once testing is successful:

git checkout main
git merge testing
git push origin main

---

✅ KEY TIPS FOR OJT TEAM
- Always work in your feature branch
- Stash before switching branches
- Pull updates before starting work
- Commit often → small logical steps
- Use testing branch for combined changes before main
- Do not push directly to main

---

💡 QUICK REFERENCE COMMANDS

git status        # check branch status
git log --oneline # view commits
git branch        # list branches
git checkout name # switch branch
git stash         # save uncommitted changes
git stash apply   # restore stashed changes
git pull origin branch
git push origin branch
git merge branch  # merge into current branch

=============================
END OF OJT GIT CHEAT SHEET
=============================