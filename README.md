# Git & GitHub
Learning Github / Git workflow

## What is GitHub?

GitHub is a place where you are able to store, share and collaborate with others on project and code. 

GitHub is free to use and is one of many places where code can be stored online for free. We use GitHub to store code as a backup, over time you will have many projects and code bases that will end up taking lots of space on your machine, its also a place where you can backup your code. Should your computer hard drive or SSD ever go corrupt your code is safe in GitHub.

## What is Git?

Git is a version control system, its a way for us to track changes in our code locally, manage a project locally and many other things. Git and Github are in no way connected to one another rather they are two separate tools. Git is a way to track, save and manage changes within your code and Github is a place where you can safely store your code as a backup. Git is a CLI tool while Github is a web application / collaborative space for developers.

NOTE: Other than Github there are other platforms like it such as GitLab, BitBucket ect. All of them server the same purpose with slight variations in what the platform offers as extra features. Through out our journey however we will stick to using GitHub, but feel free to use whatever you want!

## Terminology

- repository → The "directory" or folder that contains the code, but is tracked by Git
- remote → A repository on GitHub (or on another machine / server)
- branch → A split from the current branch, allows for new features without altering the functioning code in a code base
- un-tracked → New file / directory that is not tracked by Git
- tracked → Changes are being tracked by Git
- staged → The file(s) is added but the changes have not been committed (saved) yet
- commit → All changes are saved and a 'snapshot' is made of the current state of the code (on your local machine)
- push → Push the changes (commits) to the origin (local repository) or remote repository
- pull → Pull changes from a remote to your local repository (will pull the changes to the matching branch; main (remote) → main (local))

## Setting up git for the first time

```bash
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

the above commands need to be ran once in order to use git properly. Be sure to replace "John Doe" with your name and the email "johndoe@example.com" with your email

- Git first time setup

    [Git - First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

## Common Git commands

```bash
git clone <link>
```

clone / download a repo (project) onto your computer, in the current directory / folder you are in

EX: `git clone [https://github.com/Machine-Academy/git-workflow.git](https://github.com/Machine-Academy/git-workflow.git)`

```bash
git add .
```

add all changed files and folders, in the current folder you are in, into the `staging` area

ex: git add .

NOTE: . (dot) represents the current directory / folder that you are in.

```bash
git add fileName [file2, file3 ....]
```

add individual file(s) to the staging area, to be committed

```bash
git commit -m "commit message"

# Optionally for Git clout
git commit -m "commit type: general message

details about the commit here"
```

- Git Commits: Semantic Commits

    [Semantic Commit Messages](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716)

When you commit code, you need to create a message, these messages are very useful for your self and others to understand changes that were made in the code at the specific point in time. This is really useful for when you want to `rollback` changes you made in your project

```bash
git push origin <branch>
```

Push code back up to GitHub in the specified branch

ex: git push origin main OR git push origin dev

```bash
git checkout -b <branch name> 
```

create and move into a new branch

ex: git checkout -b testing (create a new branch called testing an move into it)

```bash
git checkout <existing branch>
```

Change your working branch, to a already existing branch.

ex: git checkout dev (change to the existing branch named "dev") OR git checkout main (change to the existing branch named "main")

```bash
git log
```

Show the commit history of the repo (project)

```bash
git pull
```

pull new code down from remote repository (GitHub repo) into the current branch you are in.

```bash
man git
```

---

## A Visual Aid

![Git%20GitHub%20workflow%201eef524eac74448ab744dad0cb0dacac/vcs.jpeg](Git%20GitHub%20workflow%201eef524eac74448ab744dad0cb0dacac/vcs.jpeg)

Or another example with a cloud based service such as GitHub:

![Git%20GitHub%20workflow%201eef524eac74448ab744dad0cb0dacac/git_in_github_overview.png](Git%20GitHub%20workflow%201eef524eac74448ab744dad0cb0dacac/git_in_github_overview.png)

## Videos

- Web Dev Simplified

    [Learn Git in 20 Minutes](https://www.youtube.com/watch?v=IHaTbJPdB-s)

- Fireship

    [Git It? How to use Git and Github](https://www.youtube.com/watch?v=HkdAHXoRtos)

- Brad Traversy

    [Git & GitHub Crash Course For Beginners](https://www.youtube.com/watch?v=SWYqp7iY_Tc)

- Learn Code Academy

    [Github Tutorial For Beginners - Github Basics for Mac or Windows & Source Control Basics](https://www.youtube.com/watch?v=0fKg7e37bQE)

## Web Resources

- [Web app for git commands / help](https://gitexplorer.com/)

