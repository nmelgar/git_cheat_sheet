# Git Cheat Sheet
Learn about Git by reading and consulting this cheat sheet.
***
<p>Changes are being made to improve it. <a target="_blank" href="#">here</a>. Feel free to contact me with suggestions.</p>

***
## Elements covered in this cheat sheet

<ul>
    <a href="#"><li>About Git</li></a>
    <a href="#"><li>Git Workflow (simplified)</li></a>
    <a href="#"><li>Git Illustrated</li></a>
    <a href="#"><li>Git commands</li></a>
    <a href="#"><li>Common Git commands</li></a>
    
</ul>

***

## About Git
|  Element  | Description   |
| --------- | ------------- |
| **What is Git?** | Git is a distributed version control system that allows you to track changes to files over time. It's designed to be fast, scalable, and ideal for both small and large projects. |
| **Local Repository** | With Git, you start by creating a local repository on your machine. This repository contains all the files and the complete history of changes made to those files. |
| **Commits** | As you make changes to your files, Git allows you to create commits. A commit is a snapshot of the changes you've made at a particular point in time. Each commit has a unique identifier called a commit hash. |
| **Branches** | Branches, are separate lines of development. They enable you to work on different features or bug fixes without affecting the main codebase. You can switch between branches and merge changes from one branch to another. |
| **Staging Area** | Git has a staging area, also known as the index, where you can choose which changes to include in your next commit. This allows you to have more control over what gets committed. |
| **Remote Repository** | A remote repository is a Git repository hosted on a remote server. GitHub is a popular platform for hosting remote repositories. It provides additional collaboration features and a web-based interface for managing Git repositories. |
| **GitHub** | GitHub is a web-based platform that uses Git for version control. It offers a graphical interface to interact with Git repositories, making it easier to collaborate with others. GitHub allows you to host your remote repositories, share code with others, and contribute to open-source projects. |
| **Pushing and Pulling** | To synchronize your local repository with a remote repository on GitHub, you use the git push command to upload your local commits. Conversely, you use the git pull command to fetch and merge the latest changes from the remote repository to your local repository. |

***

## Git workflow (simplified) 
|  Step  | Description |
| ------ | ----------- |
| **1.** | Initialize a Git repository on your local machine using **git init**. |
| **2.** | Make changes to your files and use **git add** to stage the changes. |
| **3.** | Create a commit using **git commit** to save the staged changes with a commit message. |
| **4.** | Push your commits to a remote repository on GitHub using **git push**. |
| **5.** | Collaborate with others by cloning their remote repositories using **git clone** or by creating branches, making changes, and merging them back using **git pull** and **git merge**.  |
<p>Git and GitHub provide a powerful and flexible version control system. This is just a high-level overview, there are many additional concepts and commands in Git that can be explored in more detail. </p>

***

##  Git Illustrated

![Git_Illustrated_image](https://raw.githubusercontent.com/nmelgar/git_cheat_sheet/main/images/git_illustrated.png)

***

## Git commands
<p>Git has a collection of commands that you can use to perform different tasks. Each
command serves a specific function, like creating a new repository, tracking changes,
merging code, and more.</p>
<br>
<p>Git commands has subcommands and options:</p>
<br>
<p>**Subcommands:** An additional keyword that follows the main Git command. It specifies a
specific action or operation you want to perform with that command. They
allow you to extend the functionality of the main command by defining
different tasks/actions related to it.
<br>
e.g. in the command **git remote add**, remote is the main command, and
add is the subcommand.
</p>
<br>
<p>**Option:** AKA a flag or switch, is used to modify the behavior of a Git command.
Usually represented by a hyphen (-) followed by a single character or a
double hyphen (--) followed by a descriptive name. They are used to modify
how the command operates without changing its core functionality.
<br>
e.g. in the **command git remote -v**, -v is the option. It specifies the "verbose" output and instructs Git to provide more detailed information along with the default output.
</p>

***

## Author
---
* Nefi Melgar (nefimelgarg@gmail.com)