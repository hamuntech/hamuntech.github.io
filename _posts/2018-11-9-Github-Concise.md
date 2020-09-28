---
layout: post
title: A Concise Guide to Git from Command Line
---
&lt; &gt;
* Go to the <a href="https://git-scm.com"> git website</a> and download git for your operating system
* Open the command line terminal on your machine and execute following commands. I will be using commands specific to the default OSX terminal. Please use the corresponding file system commands for your operating system.
    - <code>pwd</code> to “print working directory”. This will show your current directory.
    - In case you will like to create git repository under another directory, use the <code>cd</code> command to navigate to that directory
    - Use <code>mkdir</code> to create new directory under the main directory. This will be your local git repository
    - Use <code>cd</code> to navigate to the new directory. Currently, this directory does not have any files. So, create a file using <code>touch filename.ext</code>. Please substitute ‘filename’ with your own filename and ‘ext’ with the file extension. It can be any valid filename and extension, for example, txt, rtf, java, swift, js etc.
* To clone a remote repository on to your machine locally, you can use <code>git clone &lt;repository_url&gt;</code> or fork another repository. See <a href="https://help.github.com/articles/fork-a-repo/"> Fork a repo</a> and <a href="https://yangsu.github.io/pull-request-tutorial/"> Pull Request Tutorial</a> for details
* Now, if you execute the <code>git</code> command without any parameters, it will provide you with the command usage details
* In case you intend to exclude certain files or directories from the git process, create the .gitignore file (see details below)  before executing any git commands, as any files or directories that preexisted in the local git repository prior to creation of the .gitignore file will not be ignored. I usually prefer to execute following command before initializing a local git repository:
> <code>echo "# repository-name" >> README.md<br>
> touch LICENSE<br>
> touch .gitignore<br>
> open .gitignore</code>  (Use this command to edit the file)<br>

* To convert the current directory into a local git repository, execute <code>git init</code>
* To find out the current status of the local git repository, use <code>git status</code> command. This command will display the current branch, and to stage and discard changes from the commit operation.
* You can use either use <code>git add &lt;filename.ext&gt;</code> to add a single file, or <code>git add .</code> or <code>git add –A</code> to stage the changes to be added to the next commit operation for all files. Note that "git add ." only affects the current directory and subdirectories and "git add -A" also stages files in higher directories
* To finalize all of the changes and make them permanent in the git repository, use <code>git commit –m “your commit message”</code>
* <code>git log</code> will show the history of commits
* <code>git branch</code> will display the current branch
* You can use <code>git checkout -b &lt;new-branch-name&gt;</code> to create new branch and switch to the new branch
* To switch to another branch, use <code>git checkout < branch-name ></code>. You can also use <code>git checkout &lt;commit&gt;</code> to discard certain changes and roll back changes up to a certain point in the commit history. HEAD will move to the commit specified in git checkout. Current commit head is named HEAD (in uppercase) while the other commit heads are specified in lowercase
* To delete a branch, use <code>git branch -D &lt;branch-name&gt;</code>
* After creating a new branch and working on it, once you are ready to merge it with the master branch, first switch to the master branch using <code>git checkout master</code> and then execute the <code>git merge &lt;branch_to_be_merged&gt;</code>
* To upload your code to GitHub, first go to <a href="https://github.com"> GitHub website</a> and sign up for a free account. Follow the instructions to setup either the SSH or HTTPS method of signing into your GitHub account from the command line
* Create new repository on GitHub. You will have the option to either create a public or private repository that can optionally have a description as well as .gitignore,LICENSE.md andREADME.md files. I've reproduced post repository creation instructions below. Note that we can add the files LICENSE.md and .gitignore using the <code>touch</code> command.

## Create a new repository on the command line:
> <code>echo "# repository-name" >> README.md<br>
> git initgit add README.md<br>
> git commit -m "first commit"<br>
> git remote add origin https://github.com/username/repository-name.git<br>
> git push -u origin master</code><br>

## Push an existing repository from the command line:
> <code>git remote add origin https://github.com/username/repository-name.git<br>
> git push -u origin master</code><br>

* If you would like to obtain the exact repository URL subsequent to the initial push, click on the "Clone or download" button on the top right had side of the file listings and click on the icon next to the https URL. This will copy the git repository URL to the clipboard. Then, go back to the command line, execute the command <code>git remote add origin &lt;repository_url&gt;</code>. This will setup the remote repository.
* Use <code>git remote –v</code> to see the names git has stored for the local short name (usually origin)
* Now, you can push and pull changes to and from the remote GitHub repository using commands <code>git push &lt;remote_name&gt; &lt;remote_branch&gt;</code> and <code>git pull &lt;remote_name&gt; &lt;remote_branch&gt;</code>. For example, <code>git push origin master</code> and <code>git pull origin master</code>. You may be prompted to enter your GitHub credentials. Please see <a href="https://help.github.com/articles/which-remote-url-should-i-use/#cloning-with-https-urls-recommended"> Which remote URL should I use?</a> and <a href="https://help.github.com/articles/caching-your-github-password-in-git/"> Caching your GitHub password in Git</a> pages for details. When you execute <code>git push origin master</code> you may get a message to execute the pull first using <code>git pull origin master</code>. Once you execute <code>git pull origin master</code>, you may get the error "fatal: refusing to merge unrelated histories". In case you do get this error, you will either need to do a commit or a hard reset, using the syntax <code>git commit -m "commit message"</code> or <code>git pull origin master --allow-unrelated-histories</code> before executing <code>git pull origin master</code>. If you are prompted to explain why this merge is necessary, either type :q or :x to exit. Use <code>git status</code> to make sure that the working tree is clean and finally execute <code>git push origin master</code> to upload the repository to Github. In case you make changes to any files directly on the Github website, use <code>git pull origin master</code> to synchronize with the local repository
* To create a new branch and then pushing it to the remote repository, use <code>git checkout –b &lt;new_branch_name&gt;</code> and make whatever changes you would like to the files stored in this branch. Once you are ready to push this new branch to the remote repository, execute the <code>git push –u origin &lt;new_branch_name&gt;</code>. This will automatically link the local and remote branches. Please see <a href="https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-branch-with-git-and-manage-branches"> Create a new branch with git and manage branches</a> for details
* To remove a file from git use 'git rm'. Here is an example for a file named file1.txt:
> <code>git rm file1.txt<br>
> git commit -m "remove file1.txt"</code><br>
But if you want to remove the file only from the Git repository and not remove it from the filesystem, use:
> <code>git rm --cached file1.txt<br>
> git commit -m "remove file1.txt"</code><br>
And to push changes to remote repo:
> <code>git push origin branch_name</code><br>
(CREDIT: <a href="https://stackoverflow.com/questions/2047465/how-can-i-delete-a-file-from-git-repo">https://stackoverflow.com/questions/2047465/how-can-i-delete-a-file-from-git-repo</a>)
* In case you would like to delete your GitHub repository, open the repository and click on Settings menu on the top of the page. Scroll all the way down on the settings page to find the Delete Repository option
* To revert a local git repository back to normal directory i.e., to undo git init, use <code>rm -rf .git</code> on the command line. Use <code>git status</code> before and after this command to confirm that the operation was successful

## .gitignore file

The presence of this file in a git repository allows us to exclude any files or folders from the git repository. Any files or folders listed in this file will be ignored by git. Please note that only the files and folders added to the git repository after the creation of .gitignore file will be ignored in case they are listed in it. Any files or folders that existed in your repository prior to the creation of .gitignore file will not be ignored even if they are listed to be excluded in this file.

In case you would like to exclude a single file, just specify that file in the .gitignore file within your git repository. For example, for a file named example1.txt, just write the full filename in .gitignore as is, i.e., example1.txt.

To exclude all files with a certain extension, just write *.extension in .gitignore. For example to exclude all files with the extension of txt, write *.txt on a single line in .gitignore.

To ignore a folder, just specify the folder name followed by a slash. For example, if you would like git to ignore the contents of folder names test, then write test/ on a line in .gitignore. Please note that it works recursively. In case you would like to ignore certain type of files only in a specific folder, just prefix the file name or extension type with the folder name, separated by a slash.

A local .gitignore file in the root git repository directory can be created with the command touch .gitignore on Unix, Linux or OSX operating systems,  while a global .gitignore file to ignore certain files or folders in all git repositories on your computer, can be created with the following command:
> <code>$ git config --global core.excludesfile ~/.gitignore_global</code><br>

After creating the file, you can open it in the default text editor using open .gitignore.
Please see <a href="https://help.github.com/articles/ignoring-files/"> Ignoring files</a> for further details about ignoring files in git repositories.

Here is a template of a typical .gitignore file:
> <code>#Ignore a single fileexample1.txt<br>
> #Ignore all files with a specific extension*.txt<br>
> #Ignore the contents of a foldertest/</code><br>
