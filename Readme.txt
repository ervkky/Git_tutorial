…or create a new repository on the command line

echo "# Git_tutorial" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/ervkky/Git_tutorial.git
git push -u origin master

…or push an existing repository from the command line

git remote add origin https://github.com/ervkky/Git_tutorial.git
git branch -M master
git push -u origin master

# Deleting a Branch in Git

Using Git on your local computer allows you to delete both local and remote branches. Let's start with deleting a local branch. On the command line, you can type the following:

$ git branch -d <local-branch>

To delete a remote branch, you need to use the "git push" command:

$ git push origin --delete <remote-branch-name>

testing look like ok



