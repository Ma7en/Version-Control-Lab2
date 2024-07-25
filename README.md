# Mazen Abdeltawab Saad

# Lab2

# 1- Create a new project on your local machine, then push it your remote repo.

    -   mkdir lab2
    -   cd lab2/
    -   code .
    -   git init
    -   git add .
    -   git commit -m "first commit create"
    -   git branch -M main
    -   git remote add origin git@github.com:Ma7en/Version-Control-Lab2.git
    -   git push -u origin main

# 2- Create two branches (dev & test) then create one file on each branch, and push this changes to the remote repo.

    -   git branch dev
    -   git branch test

    -   git checkout dev
    -   => create file on branch => touch filediv.html
    -   git add .
    -   git commit -m "push file dev on branch"
    -   git push -u origin dev

    -   git checkout test
    -   => create file on branch => touch filetest.html
    -   git add .
    -   git commit -m "push file dev on branch"
    -   git push -u origin test

# 3- Merge this changes on Main branch and then push it to your remote main branch.

    -   git checkout main
    -   git merge dev
    -   git merge test
    -   git push -u origin main

# 4- how to remove them locally and remotely.

    -locally
        -   git branch -d dev
        -   git branch -d test

    -remotely
        -   git push origin :dev
        -   git push origin :test

# 5- how to checkout another branch without commit changes

    -   git stash

# 6- Create an annotated tag with tagname (v1.7).

    -   git tag -a v1.7 -m "Version 1.7"

# 7- Push it to the remote repository.

    -   git push origin v1.7
    -   git push --tags

# 8- Tell me how to list tags.

    -  git tag

# 9- Tell me how to delete tag locally and remotely.

    -   To delete local tags
        -   git tag -d v1.7

    -   To delete remote tag
        -   git push origin --delete v1.7

# 10- Add an image in the README.md file.

![Alt-text-images](./image/image-1.jpg)
