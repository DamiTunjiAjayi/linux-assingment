# Command Line Steps for My Assignment

This document outlines all the command-line steps I used from the beginning to the end to create this project. 
Each step corresponds to a commit in my Git history.

## I used my MacBook Terminal for this assignment
Set Up Project Folder and Initialize Git 
Note: Git does not track empty directories. 
I added placeholder files (.gitfile) so that the directories are included.

cd /Users/damilaretunji-ajayi/Documents/M4ACE

git init

mkdir projects

touch projects/.gitfile

git add .

git commit -m "Step 1: Create directory structure projects"

cd /Users/damilaretunji-ajayi/Documents/M4ACE/projects

mkdir week1 week2

touch week1/.gitfile week2/.gitfile

git add .

git commit -m "Step 2: Create directory structure (week1, week2) subfolder files"

cd week1

touch hello.txt

git add hello.txt

git commit -m "Step 3: Add empty file hello.txt in week1"

cd ..
cp week1/hello.txt week2/hello_copy.txt

git add week2/hello_copy.txt

git commit -m "Step 4: Copy hello.txt to week2 as hello_copy.txt"

rm week1/hello.txt

git add -u

git commit -m "Step 5: Remove original hello.txt from week1"

vim about_me.txt

git add about_me.txt

git commit -m "Step 6: Add about_me.txt with motivation for learning Node.js"

git remote add origin https://github.com/DamiTunjiAjayi/linux-assingment.git

git branch -M main

git push -f origin main
