# How-to-upload-projects-on-github
How to upload projects on github

Setting your Git username for every repository on your computer
1.	Open Git Bash.
2.	Configure git:
$ git config --global user.name "Mona Lisa"
$ git config --global user.email "Mona@gmail.com"
Confirm that you have set the Git username correctly:
3.	$ git config --global user.name
> Mona Lisa
Putting your existing work on GitHub can let you share and collaborate in lots of great ways.
4.	Initialize the local directory as a Git repository.
$ git init
1.	Add the files in your new local repository. This stages them for the first commit.
2.	$ git add .
# Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.
3.	Commit the files that you've staged in your local repository.
4.	$ git commit -m "First commit"
# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.
5.	$ git status
6.	At the top of your GitHub repository's Quick Setup page, click  to copy the remote repository URL.
  
7.	In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
8.	$ git remote add origin remote repository URL
9.	# Sets the new remote
      $git remote add origin https://github.com/boussara/test.git
# Verifies the new remote URL
Push the changes in your local repository to GitHub.
10.	$ git push origin master
# Pushes the changes in your local repository up to the remote repository you specified as

The first extra argument to git pull tells it which remote to give to the fetch operation:

 11.  $git pull origin
 
 For removing the file or folder :
 git rm -r --cached name of folder
 git commit -m 'remove folder'
 git push origin master
 then remove from the master folder
12. To show hidden files
  ls -la
13. to show the commit
  git log

git checkout <comit id>

to add new branch name
git checkout -b new name
git branch
git branch -a
git checkout -b 'correct' 'origin/correct'

Before creating a new branch, pull the changes from upstream. Your master needs to be up to date.

$ git pull
Create the branch on your local machine and switch in this branch :

$ git checkout -b [name_of_your_new_branch]
Push the branch on github :

$ git push origin [name_of_your_new_branch]
When you want to commit something in your branch, be sure to be in your branch. Add -u parameter to set upstream.

You can see all branches created by using :

$ git branch -a
Which will show :

* approval_messages
  master
  master_clean
Add a new remote for your branch :

$ git remote add [name_of_your_remote] [name_of_your_new_branch]
Push changes from your commit into your branch :

$ git push [name_of_your_new_remote] [url]
Update your branch when the original branch from official repository has been updated :

$ git fetch [name_of_your_remote]
Then you need to apply to merge changes, if your branch is derivated from develop you need to do :

$ git merge [name_of_your_remote]/develop
Delete a branch on your local filesystem :

$ git branch -d [name_of_your_new_branch]
To force the deletion of local branch on your filesystem :

$ git branch -D [name_of_your_new_branch]
Delete the branch on github :

$ git push origin :[name_of_your_new_branch]
The only difference is the : to say delete, you can do it too by using github interface to remove branch : https://help.github.com/articles/deleting-unused-branches.

If you want to change default branch, it's so easy with github, in your fork go into Admin and in the drop-down list default branch choose what you want.

If you want create a new branch:

$ git branch <name_of_your_new_branch>
