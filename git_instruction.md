# GIT INSTRUCTION
## How to work with Git.
Git - is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
![Git icon](git_image.png)
## Initialization of a new repository:
If you want to place a project under revision control, you should type the following command:

    git init

## Adding files:
If you want to add new or changed files in your working directory to the Git staging area, you should type the following command:

    git add

## Checking the status of the file:
If you want to check whether there exist some changes that you can add and commit (the command is extremely helpful when you are not sure whether you included something new to the file or whether you added it to Git), type:

    git status 

## Saving changes to Git:
If you want to save current amendment to the project history in Git, you should type the following command:

    git commit
It is always better to add to every your commit a massage that shows the user what was chnged comparing with the previous version of the file. You should type the same command but with addition  **-m "_some massage_"**:

    git commit -m "massage"

## Looking at all the commits:
To see all the versions of your project, type the following command (it will show you how each commit is named in the system and how you can refer to it while accessing the particular commit):

    git log

## Accessing particular version:
If you want to return to particular version of the project you should type the following command and add the name of the commit (which you can see after typing **git log**) or the first 4 symbols:


    git checkout <name of the version>

## To see the difference:
If you want to see the difference between sets of something, you should type this command:

    git diff
By default **git diff** shows any uncommitted changes since the last commit.

For difference between two commits you should type:

    git diff <name of version> <name of version>

## Working with remote repository:
Currently your repository is located on your device and you can access it only from it. In order to turn it into a remote repository, which you and your colleges can access in any time and from anywhere, you should upload it to your GitHub account. To do this use this commands: 

    git remote add origin <URL>
URL is given to every remote repository created by you on your GitHub WebPage. You should create a repository, copy its URL and paste it in the <...> in the command.
After that you should type two more commands:

    git branch -M main

    git push -u origin main
Now everything from your local file is transfered to remote repository. But if you add something in the local one new information is not automatically transfered to the remote repository. In order to do this you should type the following command:

    git push
this command pushes your local commits to remote repository.

If something was added in your remote repository it also will not be automatically transfered to your local one. You should use the following command:

    git push
this command pulls added information from your remote repository.