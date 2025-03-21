…or create a new repository on the command line




///////////////////////////////////////////////////////////////////////////////////////////
<<<<<<< HEAD
=======
git set/check and verigy remote
git remote -v ////////Verify new remote URL
git remote show origin////////////To see which remote URL you have currently in this local repository: 
git remote set-url origin githubrepurl///////////////For adding or changing the remote origin:
git push -u origin master/////specify upstream to set-url
for pull new repository and to add origin
git init
git remote add origin https://github.com/ervkky/Timer_No_RTC
git fetch origin///////////fetch master
git checkout main////////////switch branch to main
git pull origin main//////pull verify main
If you cloned the repository directly using git clone <repository-URL>,
 you can skip steps 1 and 2 and directly run step 5. 



>>>>>>> master

git procedure
$ git config --global user.name "Your Name Comes Here"
$ git config --global user.email you@yourdomain.example.com

Initialized empty Git repository in .git/
$ git init
Next, tell Git to take a snapshot of the contents of all files under the current directory (note the .), 
with git add:
$ git add .
You can permanently store the contents of the index in the repository with git commit:
$ git commit -m "message"
You can also get a brief summary of the situation with git status:
$ git status
At any point you can view the history of your changes using
$ git log
$ git log -p
$ git log --stat --summary
/////////////////////////////////////////////////////////////////////////////////////

////////////////////////////////////////////////////GIT-Bracnch///////////////////////
 To create a new branch named experimental, use
$ git branch experimental
If you now run
$ git branch
you’ll get a list of all existing branches:

  experimental
* master

The experimental branch is the one you just created, and the master branch is a default branch that was created for you automatically. The asterisk marks the branch you are currently on; type

$ git switch experimental

to switch to the experimental branch. Now edit a file, commit the change, and switch back to the master branch:

(edit file)
$ git commit -a
$ git switch master

Check that the change you made is no longer visible, since it was made on the experimental branch and you’re back on the master branch.






Show all existing branch in git
$ git branch
change branch
$ git checkout branchName
echo "# Git_tutorial" >> README.md
git init
git add README.md
git add .///////////before adding commit
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/ervkky/Git_tutorial.git
git push -u origin master

…or push an existing repository from the command line

git remote add origin https://github.com/ervkky/Git_tutorial.git
git branch -M master
git push -u origin master


# Git Branch operation
show current branch
$ git branch --show
show all branch
git show-branch [-a | --all] [-r | --remotes] [--topo-order | --date-order]
		[--current] [--color[=<when>] | --no-color] [--sparse]
		[--more=<n> | --list | --independent | --merge-base]
		[--no-name | --sha1-name] [--topics]
		[(<rev> | <glob>)…​]
git show-branch (-g | --reflog)[=<n>[,<base>]] [--list] [<ref>]
# Deleting a Branch in Git

Using Git on your local computer allows you to delete both local and remote branches. Let's start with deleting a local branch. On the command line, you can type the following:

$ git branch -d <local-branch>

TO Rename existing Branch
Rename the current branch: & git branch -m new-branch-name
Rename a specific branch: git branch -m old-branch-name new-branch-name


To propagate the change to a remote, you can use git push to push the new branch and delete the old branch:

    git push origin -u new-branch-name
    git push origin --delete old-branch-name

To delete a remote branch, you need to use the "git push" command:

$ git push origin --delete <remote-branch-name>

To Archive git project
		<b>Archiving the HEAD commit<b>
$ git archive --format=tar HEAD > project.tar
		OR
$ git archive --format=tar HEAD > project.tar
		Archiving a specific branch or tag
$ git archive --format=zip feature-xyz > feature-xys.zip
	Archiving a specific folder
$ git archive --format=zip --output=src.zip HEAD src/
	Archiving a remote Git repository
$ git archive --remote=https://example.com/myrepo.git main | gzip > myrepo-main.zip
	


 



