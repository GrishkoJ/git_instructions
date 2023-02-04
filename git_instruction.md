# GIT INSTRUCTION
## How to work with Git.
Git - is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

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

