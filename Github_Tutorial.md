# Version Control: The Basics of Github

According to Wikipedia, Github is a "web based version control repository."
In simple English, that means that Github is an online service that allows you to track and merge changes you and your teammates have made to your work. Github also allows you to do lots of other cool things, like host websites, make a Trello-like project board, and write documentation on your work.

Let’s start with the basics.

## Step by step: How to save your files on Github

1. [git clone](https://git-scm.com/docs/git-clone): (Only use this command the first time you want to access a repository) Copies the specified repository to your computer. 

    1. `git clone <insert repository URL here>`

    2. ![git_clone](https://github.com/Oktober13/Tutorials/blob/master/images/github_tut/git_visual_Page_1.png)

2. [git pull](https://git-scm.com/docs/git-pull): Updates your local copy of the repository, on your computer.

    1. General command: `git pull`

    2. Pulling specific branch: ’git pull origin <remote branchname>’

    3. ![git_pull](https://github.com/Oktober13/Tutorials/blob/master/images/github_tut/git_visual_Page_3.png)

3. [git add](https://git-scm.com/docs/git-add): Adds <filename’s> contents to the index of files being pushed to Github.

    1. Command: `git add`

4. [git commit](https://git-scm.com/docs/git-commit): Stores all indexed files in a new commit, and tags them with a log message from the user, describing all changes.

    1. Command: `git commit`

    2. ![git_add_commit](https://github.com/Oktober13/Tutorials/blob/master/images/github_tut/git_visual_Page_5.png)

5. [git push](https://git-scm.com/docs/git-push): Updates all remote repositories based on the files that were commited

    1. General command: `git push`

    2. Specific branch: `git push < remote_repository_name > < branch_name >

    3. ![git_push](https://github.com/Oktober13/Tutorials/blob/master//images/github_tut/git_visual_Page_7.png)

6. Git pull request: Lets the repository owner know that they should merge your changes with the master branch

    1. How to make a pull request: [https://help.github.com/articles/creating-a-pull-request/](https://help.github.com/articles/creating-a-pull-request/)

    2. ![git_pullrequest](https://github.com/Oktober13/Tutorials/blob/master/images/github_tut/git_visual_Page_8.png)

## How to push a file to Github (short version):

1. `git add <filename>`

2. `git commit –m “< insert commit message >”`

3. `git push origin <branchname>`

## Assorted Useful Git commands:

1. [git branch](https://git-scm.com/docs/git-branch): Creates a new branch, or version of the code, by duplicating your current pushed version of the code. You can now work off of the code in the new branch and implement different functionality.

    1. ![git_branch](https://github.com/Oktober13/Tutorials/blob/master/images/github_tut/git_visual_Page_2.png)

2. [git stash](https://git-scm.com/docs/git-stash): Saves your currently commited, but not pushed, files in a “stash,” where they can later be accessed if needed. “Git Stash Apply” reverses this process.

    1. `git stash < stash_name >`

    2. `git stash apply < stash_name >`
    
    3. ![git_stash](https://github.com/Oktober13/Tutorials/blob/master/images/github_tut/git_visual_Page_6.png)

3. [git status](https://git-scm.com/docs/git-status): Tells you what files are currently commited and will be pushed to Github.

    1. `git status`

## References: 

• Repository: The overarching location where code is stored for a project/etc.

• [Remote repository](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes): Versions of your repository hosted elsewhere on the internet. They enable you to collaborate and share work with others.

• Branch: The “folder” containing a particular version of your code. You can only work on one branch at a time.

• Master branch: The branch containing the “official” version of the code. You should only push working code to the master branch, so that this version of code is functional at all times.

• [Merge conflict](https://githowto.com/resolving_conflicts): An error that occurs when you edit the same file as someone else, then try to push your changes. Github isn’t sure which version is correct, so you must go back and manually determine which changes should be preserved.

• [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet): A “coding language” specific to Github wikis and webpages. It uses specific syntax to encode graphics.

• < Stuff >: The convention for marking user-specific input. Insert whatever “Stuff” is here. Don’t leave the “<>” signs in when executing the command.

*This tutorial was written by [L. Zuehsow](https://github.com/Oktober13), on 2-25-17. This page can also be found on the Olin Robotics webpage at olinrobotics.github.io .*
