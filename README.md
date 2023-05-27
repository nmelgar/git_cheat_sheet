# Git Cheat Sheet
Learn about Git by reading and consulting this cheat sheet.
***
<p>Changes are being made to improve it. <a target="_blank" href="#">here</a>. Feel free to contact me with suggestions.</p>

***
## Elements covered in this cheat sheet

<ul>
    <a href="#about-git"><li>About Git</li></a>
    <a href="#git-workflow"><li>Git Workflow (simplified)</li></a>
    <a href="#git-illustrated"><li>Git Illustrated</li></a>
    <a href="#git-commands"><li>Git commands</li></a>
    <a href="#git-common-c"><li>Common Git commands</li></a>
    
</ul>

***

## About Git<a name="about-git"></a>
|  Element  | Description   |
| --------- | ------------- |
| __What is Git?__ | Git is a distributed version control system that allows you to track changes to files over time. It's designed to be fast, scalable, and ideal for both small and large projects. |
| __Local Repository__ | With Git, you start by creating a local repository on your machine. This repository contains all the files and the complete history of changes made to those files. |
| __Commits__ | As you make changes to your files, Git allows you to create commits. A commit is a snapshot of the changes you've made at a particular point in time. Each commit has a unique identifier called a commit hash. |
| __Branches__ | Branches, are separate lines of development. They enable you to work on different features or bug fixes without affecting the main codebase. You can switch between branches and merge changes from one branch to another. |
| __Staging Area__* | Git has a staging area, also known as the index, where you can choose which changes to include in your next commit. This allows you to have more control over what gets committed. |
| __Remote Repository__ | A remote repository is a Git repository hosted on a remote server. GitHub is a popular platform for hosting remote repositories. It provides additional collaboration features and a web-based interface for managing Git repositories. |
| __GitHub__ | GitHub is a web-based platform that uses Git for version control. It offers a graphical interface to interact with Git repositories, making it easier to collaborate with others. GitHub allows you to host your remote repositories, share code with others, and contribute to open-source projects. |
| __Pushing and Pulling__ | To synchronize your local repository with a remote repository on GitHub, you use the git push command to upload your local commits. Conversely, you use the git pull command to fetch and merge the latest changes from the remote repository to your local repository. |

***

## Git workflow (simplified)<a name="git-workflow"></a>
|  Step  | Description |
| ------ | ----------- |
| __1.__ | Initialize a Git repository on your local machine using __git init__. |
| __2.__ | Make changes to your files and use __git add__ to stage the changes. |
| __3.__ | Create a commit using __git commit__ to save the staged changes with a commit message. |
| __4.__ | Push your commits to a remote repository on GitHub using __git push__. |
| __5.__ | Collaborate with others by cloning their remote repositories using __git clone__ or by creating branches, making changes, and merging them back using __git pull__ and __git merge__.  |
<p>Git and GitHub provide a powerful and flexible version control system. This is just a high-level overview, there are many additional concepts and commands in Git that can be explored in more detail. </p>

***

##  Git Illustrated<a name="git-illustrated"></a>

![Git_Illustrated_image](https://raw.githubusercontent.com/nmelgar/git_cheat_sheet/main/images/git_illustrated.png)

***

## Git commands<a name="git-commands"></a>

<p>Git has a collection of commands that you can use to perform different tasks. Each
command serves a specific function, like creating a new repository, tracking changes,
merging code, and more.</p>

<p>Git commands has subcommands and options:</p>

| Element | Description |
| ------- | ----------- |
| __Subcommands__ | An additional keyword that follows the main Git command. It specifies a specific action or operation you want to perform with that command. They allow you to extend the functionality of the main command by defining different tasks/actions related to it.<br>e.g. in the command __git remote add__, remote is the main command, and add is the subcommand.|
| __Option__ | AKA a flag or switch, is used to modify the behavior of a Git command. Usually represented by a hyphen (-) followed by a single character or a double hyphen (--) followed by a descriptive name. They are used to modify how the command operates without changing its core functionality.<br>e.g. in the **command git remote -v**, -v is the option. It specifies the "verbose" output and instructs Git to provide more detailed information along with the default output. |

***

## Common Git commands<a name="git-common-c"></a>

| Command | Description + Example |
| ------- | --------------------- |
| __git init__ | Initializes a new Git repository in the current directory.<br>__git init__ -> creates a new empty Git repository. |
| __git clone__ | Copies a remote repository and sets it up locally.<br>__git clone <repository_url>__ -> clones the remote repository specified by <repository_url> to your local machine. |
| __git add__ | Adds changes or new files to the staging area.<br>__git add <file_name>__ -> stages the changes made to <file_name> for the next commit. |
| __git commit__ | Records the changes to the repository.<br>__git commit -m__ "Commit message" -> commits the staged changes with the provided commit message. |
| __git push__ | Uploads the local commits to a remote repository.<br>__git push origin master__ -> pushes the commits from the local "master" branch to the remote repository named "origin." |
| __git pull__ | Fetches changes from a remote repository and integrates them into the current branch.<br>__git pull origin master__ -> fetches changes from the remote repository named "origin" and merges them into the local "master" branch. |
| __git branch__ | Lists, creates, or deletes branches.<br>__git branch__ -> lists all the branches in the repository. |
| __git checkout__ | Switches between branches or restores files from a previous commit.<br>__git checkout <branch_name>__ -> switches to the branch specified by <branch_name>. |
| __git merge__| Combines changes from different branches.<br>__git merge <branch_name>__ -> merges the changes from <branch_name> into the current branch. |
| __git status__| Shows the current state of the repository.<br>__git status__ -> displays information about the modified, staged, and untracked files in the repository. |
| __git log__ | Displays the commit history of the repository.<br>__git log__ -> shows a chronological list of commits, including commit hashes, authors, dates, and commit messages.|
| __git diff__ | Shows the differences between the current state and previous commits or between branches.<br>__git diff__ -> displays the changes made to the files in the current working directory compared to the last commit. |
| __stash__ | Temporarily saves changes that are not ready to be committed.<br>__git stash save "feature in progress"__ -> stores the current changes in a stash with the provided message. |
| __git remote__ | Manages remote repositories.<br>__git remote -v__ -> lists the configured remote repositories and their URLs.<br>__git remote add <remote_name> <repository_url>__ -> adds a new remote repository. |
| __git fetch__ | Downloads the latest changes from a remote repository without merging them.<br>__git fetch origin__ -> fetches the latest changes from the remote repository named "origin" without merging them into the local branch. |
| __git reset__ | Undoes commits by moving the branch pointer backward.<br>__git reset HEAD~1__ -> undoes the last commit and moves the branch pointer one commit back (HEAD~1 refers to the commit one step before). |
| __git rebase__ | Applies changes from one branch onto another branch.<br>__git rebase <branch_name>__ -> incorporates the changes from <branch_name> onto the current branch. |
| __git blame__ | Shows who last modified each line of a file.<b>__git blame <file_name>__ -> displays the author and commit information for each line of <file_name>. |
| __git config__ | Sets up Git configuration variables.<br>__git config --global user.name "John Doe"__ -> sets the global username to "John Doe" for all Git repositories on your machine. |

***

## Author
---
* Nefi Melgar (nefimelgarg@gmail.com)