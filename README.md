# GIT MAIN COMMANDS 

# Moving around tree + infos
git status  

git log 

git checkout -b branch_name //-b create a new branch

git merge branch_name --no-commit //Then check and commit



# Create a new repository on the command line
echo "# GIT" >> README.md

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin https://github.com/BaptisteB142/GIT.git

git push -u origin main

# push an existing repository from the command line
git remote add origin https://github.com/BaptisteB142/GIT.git

git branch -M main

git push -u origin main
