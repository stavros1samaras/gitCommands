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

git init

git remote add origin <URL_of_your_Repo>

git add .

git commit -m "Local changes"

git branch -M main

git push -u origin main

## 4. Clone an Existing Repo from GitHub
### Copy a repo to a new local folder

git clone <URL_of_your_Repo>

cd <folder_name>

git add .

git commit -m "My changes"

git push -u origin main


# Βranches

#### συνδεω γκιτ με γκιτχαμπ αλλιως δεν εχω μπραντσις
git remote add origin https://github.com/stavros1samaras/gitExample.git

git add .

git commit -m "first commit"

#### κανω push -u γιατι ειναι η πρωτη φορα που κανω push

git push -u origin main

#### αλλαζω branch και το δημιουργω ταυτοχρωνα

git switch -c temp

git add readMe2.txt

git commit -m "readMe2 added"

#### ξανα κανω push -u γιατι ειναι η πρωτη φορα που κανω push στο temp branch

git push -u origin temp

#### εδω βλεπω τα 2 branches μου main και temp
git branch

git switch main

#### αυτο ειναι το ιστορικο του branch
git log --oneline



