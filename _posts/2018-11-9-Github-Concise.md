---
layout: post
title: A Concise Guide to Git from Command Line
---

* Go to the <a href="https://git-scm.com"> git website</a> and download git for your operating system
* Open the command line terminal on your machine and execute following commands. I will be using commands specific to the default OSX terminal. Please use the corresponding file system commands for your operating system.
    - pwd to “print working directory”. This will show your current directory.
    - In case you will like to create git repository under another directory, use the cd command to navigate to that directory
    - Use mkdir to create new directory under the main directory. This will be your local git repository
    - Use cd to navigate to the new directory. Currently, this directory does not have any files. So, create a file using touch filename.ext. Please substitute ‘filename’ with your own filename and ‘ext’ with the file extension. It can be any valid filename and extension, for example, txt, rtf, java, swift, js etc.
* To clone a remote repository on to your machine locally, you can use git clone <repository_url> or fork another repository. <a href="https://help.github.com/articles/fork-a-repo/"> Fork a repo</a> and <a href="https://yangsu.github.io/pull-request-tutorial/"> Pull Request Tutorial</a> for details
* Now, if you execute the command git without any parameters, it will provide you with the command usage details
* In case you intend to exclude certain files or directories from the git process, create the .gitignore file (see details below)  before executing any git commands, as any files or directories that preexisted in the local git repository prior to creation of the .gitignore file will not be ignored. I usually prefer to execute following command before initializing a local git repository:
<p><code>echo "# repository-name" >> README.md
touch LICENSE
touch .gitignore
open .gitignore</code>  (Use this command to edit the file)</p>
To convert the current directory into a local git repository, execute git init
To find out the current status of the local git repository, use git status command. This command will display the current branch, and to stage and discard changes from the commit operation.
You can use either use git add <filename.ext> to add a single file, or git add . or git add –A to stage the changes to be added to the next commit operation for all files. Note that "git add ." only affects the current directory and subdirectories and "git add -A" also stages files in higher directories
To finalize all of the changes and make them permanent in the git repository, use git commit –m “your commit message”
git log will show the history of commits
git branch will display the current branch
You can use git checkout -b <new-branch-name> to create new branch and switch to the new branch
To switch to another branch, use git checkout < branch-name >. You can also use git checkout <commit> to discard certain changes and roll back changes up to a certain point in the commit history. HEAD will move to the commit specified in git checkout. Current commit head is named HEAD (in uppercase) while the other commit heads are specified in lowercase
To delete a branch, use git branch -D <branch-name>
After creating a new branch and working o it once you are ready to merge it with the master branch, first switch to the master branch using git checkout master and then execute the git merge <branch_to_be_merged>
To upload your code to GitHub, first go to GitHub website and sign up for a free account. Follow the instructions to setup either the SSH or HTTPS method of signing into your GitHub account from the command line
Create new repository on GitHub. You will have the option to either create a public or private repository that can optionally have a description as well as .gitignore,LICENSE.md andREADME.md files. I've reproduced post repository creation instructions below. Note that we can add the files LICENSE.md and .gitignore using the touch command.
Create a new repository on the command line:
echo "# repository-name" >> README.mdgit initgit add README.mdgit commit -m "first commit"git remote add origin https://github.com/username/repository-name.gitgit push -u origin master
Push an existing repository from the command line:
git remote add origin https://github.com/username/repository-name.gitgit push -u origin master

If you would like to obtain the exact repository URL subsequent to the initial push, click on the "Clone or download" button on the top right had side of the file listings and click on the icon next to the https URL. This will copy the git repository URL to the clipboard. Then, go back to the command line, execute the command git remote add origin <repository_url>. This will setup the remote repository.
Use git remote –v to see the names git has stored for the local short name (usually origin)
Now, you can push and pull changes to and from the remote GitHub repository using commands git push <remote_name> <remote_branch> and git pull <remote_name> <remote_branch>. For example, git push origin master andgit pull origin master. You may be prompted to enter your GitHub credentials. Please see Which remote URL should I use? and Caching your GitHub password in Git pages for details. When you execute git push origin masteryou may get a message to execute the pull first using git pull origin master. Once you execute git pull origin master, you may get the error fatal: refusing to merge unrelated histories. In case you do get this error, you will either need to do a commit or a hard reset, using the syntax git commit -m "commit message" or git pull origin master --allow-unrelated-histories before executing git pull origin master. If you are prompted to explain why this merge is necessary, either type :q or :x to exit. Use git statusto make sure that the working tree is clean and finally execute git push origin master to upload the repository to Github. In case you make changes to any files directly on the Github website, use git pull origin masterto synchronize with the local repository
To create a new branch and then pushing it to the remote repository, use git checkout –b <new_branch_name> and make whatever changes you would like to the files stored in this branch. Once you are ready to push this new branch to the remote repository, execute the git push –u origin <new_branch_name>. This will automatically link the local and remote branches. Please see Create a new branch with git and manage branches for details

To remove a file from git use 'git rm'. Here is an example for a file named file1.txt:
git rm file1.txtgit commit -m "remove file1.txt"
But if you want to remove the file only from the Git repository and not remove it from the filesystem, use:
git rm --cached file1.txtgit commit -m "remove file1.txt"
And to push changes to remote repo:
git push origin branch_name
(CREDIT: https://stackoverflow.com/questions/2047465/how-can-i-delete-a-file-from-git-repo)
In case you would like to delete your GitHub repository, open the repository and click on Settings menu on the top of the page. Scroll all the way down on the settings page to find the Delete Repository option
To revert a local git repository back to normal directory i.e., to undo git init, use rm -rf .git on the command line. Use git status before and after this command to confirm that the operation was successful
.gitignore file
The presence of this file in a git repository allows us to exclude any files or folders from the git repository. Any files or folders listed in this file will be ignored by git. Please note that only the files and folders added to the git repository after the creation of .gitignore file will be ignored in case they are listed in it. Any files or folders that existed in your repository prior to the creation of .gitignore file will not be ignored even if they are listed to be excluded in this file.
In case you would like to exclude a single file, just specify that file in the .gitignore file within your git repository. For example, for a file named example1.txt, just write the full filename in .gitignore as is, i.e., example1.txt.
To exclude all files with a certain extension, just write *.extension in .gitignore. For example to exclude all files with the extension of txt, write *.txt on a single line in .gitignore.
To ignore a folder, just specify the folder name followed by a slash. For example, if you would like git to ignore the contents of folder names test, then write test/ on a line in .gitignore. Please note that it works recursively. In case you would like to ignore certain type of files only in a specific folder, just prefix the file name or extension type with the folder name, separated by a slash.
A local .gitignore file in the root git repository directory can be created with the command touch .gitignore on Unix, Linux or OSX operating systems,  while a global .gitignore file to ignore certain files or folders in all git repositories on your computer, can be created with the following command:
$ git config --global core.excludesfile ~/.gitignore_global
After creating the file, you can open it in the default text editor using open .gitignore.
Please see Ignoring files for further details about ignoring files in git repositories.
Here is a template of a typical .gitignore file:
#Ignore a single fileexample1.txt
#Ignore all files with a specific extension*.txt
#Ignore the contents of a foldertest/
