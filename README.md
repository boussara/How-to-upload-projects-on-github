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
      $ git remote -v
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


