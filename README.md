how to push
fork repo dulu ygy
git init
git clone link repo
cd dulu ke folder
code .
kerjakan bagianmu
git branch namabranch ytta
git switch namabranch
git add .
if file tidak ada cd dulu ke folder repo nya
git commit -m "aku sudah kerja"
git remote add origin link repo
git push -u origin nama branch

warning!!!! 
pastikan akun github nya sudah kamu ganti
jika nyangkut sama akun lain ke control panel terus search credential manager hapus akun github orang lain
gl gl yall

How to solve this problem of "! [rejected] master -> master (fetch first)"

First Do this ...

git fetch origin master
git merge  master

Then, do this ...

git fetch origin master:tmp
git rebase tmp
git push origin HEAD:master
git branch -D tmp

kalau yang error nya main yah ganti jadi main kocak

nigga kalau akun lu nabrak
43

1- configure your new username and email with

change username: git config username.user <username>

change email: git config username.email <email>
OR
git config --global user.name "Full Name"
git config --global user.email "email@address.com"

2- run this command git commit --amend -C HEAD --reset-author

3- run this command git push --force

This will change the other in the last commit.
