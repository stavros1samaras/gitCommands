# Git Commands Cheat Sheet

## 1. Git Configuration
### Set your user name and email (only once per computer)
git config --global user.name "Your Name"

git config --global user.email "email@domain.com"

## 2. If You Already Have a Project in VSCode
### Initialize Git locally, commit your files, and push to GitHub
git init

git add .

git commit -m "YOUR MESSAGE"

git remote add origin https://github.com/stavros1samaras/[yourRepository].git

git branch -M main

git push -u origin main


## 3. Link an Existing GitHub Repo with Your Local Repo
### If the repo already exists on GitHub

cd myproject

git init

git remote add origin <URL_of_your_Repo>

git pull origin master

git add .

git commit -m "Local changes"

git push -u origin main

## 4. Clone an Existing Repo from GitHub
### Copy a repo to a new local folder

git clone <URL_of_your_Repo>

cd <folder_name>

git add .

git commit -m "My changes"

git push -u origin main

