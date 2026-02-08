# Termux Beginner Guide 

This guide is for beginners who want to learn how to use Termux on Android.  
It covers installation, basic commands, Python, Git, GitHub, Markdown, and useful tips.

## Table of Contents

- [What is Termux?](#what-is-termux)
- [1. Installation and Setup](#1-installation-and-setup)
- [2. File System Navigation](#2-file-system-navigation)
- [3. Python Basics](#3-python-basics)
- [4. Git and GitHub Basics](#4-git-and-github-basics)
- [5. Markdown for Projects](#5-markdown-for-projects)
- [6. Tips and Best Practices](#6-tips-and-best-practices)
- [7. References and Sources](#7-references-and-sources)
## What is Termux?

Termux is a terminal emulator for Android that allows you to run Linux commands and programming tools like Python and Git.  
It’s perfect for learning programming, open source contributions, and development on a mobile device.

If you don’t have Termux, download it from F-Droid : 
 [Termux](https://f-droid.org/packages/com.termux/)

### 1. Installation and Setup

1. Update packages:

```
pkg update && pkg upgrade
```

2. Install essential tools:

```
pkg install git python nano curl wget
```


3. Setup storage access:
```
termux-setup-storage
```

This allows Termux to access your files.

4. Optional: Customize your terminal with .bashrc:
```
nano ~/.bashrc
```

   Add lines like:
   ```
mkdir myprojects
cd myprojects
```

Save with CTRL + X, Y, Enter.

### 2. File System Navigation

Basic commands:

```
pwd       # Show current folder
ls        # List files
cd folder # Go to folder
mkdir newfolder
rm file
mv old new
cp file1 file2
```


Example:
```
mkdir myprojects
cd myprojects
```

### 3. Python Basics

Check Python version:
```
python --version
```

Create a file:
```
nano hello.py
`````

Write:
```
print("Hello from Termux")
name = input("What is your name? ")
print("Hello,", name)
```

Run:
```
python hello.py
```

Install additional modules:
```
pip install requests
```

### 4. Git and GitHub Basics

Check Git version:
```
git --version
```

Create a repository locally
```
mkdir myrepo
cd myrepo
git init
```

Add a file
```
touch README.md
nano README.md
```

Write some text, save, then:
```
git add .
git commit -m "Initial commit"
```
Useful Git commands
```
git status       # Check changes  
git branch       # Show branches  
git checkout -b newbranch  # Create a new branch  
git pull         # Pull changes from remote  
git merge branch_name
```
### 5. Markdown for Projects

Markdown is used for README files and documentation.

Example:

```
Markdown
# Project Title
## Description
This is my project.

### Features
- Feature 1
- Feature 2

**Bold text**  
*Italic text*  
[Link](https://example.com)
```
### 6. Tips and Best Practices

- Practice every day, even 15–30 minutes
- Don’t be afraid of mistakes; errors help you learn
- Keep projects organized in folders
- Read documentation for Python, Git, and Termux
- Ask questions on forums or GitHub if stuck
- Backup your work regularly

### 7. References and Sources

- [Termux Official Documentation](https://wiki.termux.com) – The official wiki for learning Termux commands and features.  
- [F-Droid (Termux download)](https://f-droid.org/packages/com.termux/) – Safe and official place to download Termux on Android.  
- [Git Documentation](https://git-scm.com/doc) – Official documentation for Git version control system.  
- [Python Official Docs](https://docs.python.org/3/) – Official Python documentation and tutorials.  
- [Markdown Guide](https://www.markdownguide.org/basic-syntax/) – A complete guide to Markdown syntax for writing docs and READMEs.