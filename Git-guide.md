
# Git Guide for Beginners – Commands and Workflow Step by Step

This file is part of my **Outreachy application portfolio**.  

It is designed to help complete beginners learn **Git** and **GitHub**, even with no prior experience.



## What is Git?

Git is a **version control system** that allows you to track changes in your files and collaborate with others efficiently.

With Git, you can:
- Save the history of your work  
- Go back to previous versions if something breaks  
- Work with other people without losing your changes  

 Example:  
You are working on a project and add a new feature. Git allows you to see exactly what changed since the last version.



### What is a workflow?

In Git, a **workflow** is simply **the logical order of steps you follow when working on a project**.

For a beginner, a basic workflow looks like this:
1. Create or edit a file  
2. Check the repository status (`git status`)  
3. Add the file (`git add`)  
4. Create a commit (`git commit`)  
5. Send changes to GitHub (`git push`)  

A workflow helps you work in an organized way and avoid mistakes.



### Creating a repository and understanding the workflow

A **repository** is a folder that contains:
- Your project files  
- The history of all changes made to those files  

### Step 1: Create a local repository
```bash
git init```

Initializes **Git** in the current folder
Your files can now be tracked by Git

Step 2: Check repository status

```Bash
git status```

Shows modified, added, or untracked files
Helps you know what will be included in the next commit

Adding and saving changes
Add a specific file


```Bash
git add file_name```

Prepares the file for commit

Tip: use git status to confirm it was added
Add all modified files


```Bash
git add .```

Adds all changes at once
Create a commit

```Bash
git commit -m "Clear and descriptive message"```

Example:

```Bash
git commit -m "Add Git guide for beginners"```

**Beginner tip**: Commit often with clear messages to track your progress easily.

### Sending your changes to GitHub
Connect your local repository to GitHub (one time)

```Bash
git remote add origin <repository_URL>```

Push commits to GitHub

```Bash
git push -u origin main```

Sends your commits to the remote repository
Pull updates from GitHub

```Bash
git pull```

Updates your local repository with remote changes

**Tip**: Always run git pull before starting new work to avoid conflicts.

 ### Common problems and solutions

Error: src refspec main does not match any
Cause: No commit was made before pushing
Solution: Create a commit, then push again

Error: fatal: not a git repository
Cause: You are not inside a Git repository
Solution: Initialize the folder using *git init*

### Merge conflicts
Merge conflicts happen when two branches modify the same part of a file.

To resolve a conflict:
Open the file and review the conflicting changes
Choose which version to keep
Save the file and create a new commit

**Tip**: Use branches to develop new features safely.

### Complete beginner workflow example
Example: Adding a new file to GitHub
Create a file called example.txt

Check status:

```Bash
git status```

Add the file:

```Bash
git add example.txt```

Commit the file:

```Bash
git commit -m "Add example.txt file"```

Push to GitHub:

```Bash
git push```

### Practical tips
Always check git status before adding or committing
Write short and clear commit messages
Commit frequently to avoid losing work
Use branches to experiment with new features

### Using Git on a smartphone
If you don’t have a computer, you can still use Git on Android.
Option 1: GitHub mobile app
Create and edit files directly on GitHub
Commit changes without using a terminal
Limitation: Some Git commands are not available (git init, git pull, etc.)

Option 2: Termux (recommended)
Install Termux
Install Git:

```Bash
pkg install git```

Configure your identity:

```Bash
git config --global user.name "Jukaële"
git config --global user.email "jnlouisjukaele@gmail.com"```

You can now use all Git commands (`git init`, `git add`, `git commit`, `git push`, `git pull`) directly on your phone

**Tip**: Clone your GitHub repository in Termux to edit files locally and push changes.

- **Useful resources**

Official Git documentation: https://git-scm.com/doc
Interactive guide: https://learngitbranching.js.org/
Search “Git basics” on YouTube for beginner-friendly tutorials
This guide is written to help beginners confidently use Git and build a strong Outreachy portfolio.
Copier le code


#### Next step (important)
Make **one clean commit** with a message like:
Add complete Git guide for beginners with workflow and mobile usage.