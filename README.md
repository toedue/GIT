# GIT

### . Git is a VCS. (VCS means Version Control System).

### . A VCS is like a time machine for your work (your code).

### . Commit means you are saving a point in time.


## 1. What is Git? 
Git is a tool that helps you keep track of all the changes you make to your work (like computer code, but it could be other files too).

Think of it like this: Imagine you are writing a very long school paper. Instead of just one file, you save a new copy every time you finish a big part.

    File 1: The Intro (Finished on Monday)

    File 2: Intro + Main Body (Finished on Tuesday)

    File 3: Final Draft (Finished on Wednesday)

Git does this automatically and much better. It saves every change without making many copies on your computer.

## 2. What is a "Time Machine"? 
When people say Git is like a "time machine," they mean you can always go back to an older, saved version of your work.

Example: You make a big change today, and it breaks your code. With Git, you can tell the system, "Go back to the way my code looked yesterday!" It is like pressing the rewind button.

## 3. What is a "Commit"? 
A Commit is the action of saving your progress in Git. It's like taking a snapshot of all your files at that exact moment.

When you Commit, you are telling Git:

    "I'm happy with all the changes I made since the last save."

    "Please record this moment so I can come back to it later."


## Why Git Helps You
Here are the notes for your text about Git, broken down into simple points:

    Track Changes: Git helps you see what changes you made to your code.

    Go Back in Time: You can easily return to an older, saved version of your work.

    Teamwork: It lets many people work on the same project without making a big mess.


## 1. Tracking Changes 
This means Git always remembers everything you do to your files.

Example: You delete a line of code, and then two days later, you change a word. Git keeps a full history of these steps. If you need to know exactly when or why you made a change, Git can show you.

## 2. Going Back in Time 
This is the most powerful part. Since Git saves every "commit" (your saved progress), you have many safe points you can jump back to.

Analogy: Imagine playing a video game where you can save your progress at any time. If you make a mistake in the game (or in your code), you don't have to start over. You just load the last good save point.

## 3. Teamwork without Messing Up 
Git is great when you work with others. Each person can work on their own piece of the code without breaking what others are doing.

How it works: Git has smart rules to help put everyone's separate work together. If two people change the same line of code, Git will point it out and ask them to fix the small conflict before saving the final version. This stops people from accidentally deleting or writing over each other's work.



## Git vs. GitHub 

### . Git is the tool you use on your own computer (local).

### . GitHub is a website where you keep your Git projects online (in the cloud).

### . GitHub helps you share your projects and work with others (collaborate).

### . On GitHub, you can check code (review) and find problems (trace issues).


## 1. Git (The Tool) 
Think of Git as the software you install on your laptop. It's the engine that does the actual work of saving versions and tracking changes.

Key Idea: It handles the whole "time machine" process locally (only on your machine).

## 2. GitHub (The Platform) 
GitHub is like a giant online filing cabinet or a social network for coders. It is a specific website (a platform) that holds all the projects you manage with Git.

Why use it?

    Backup: Your work is safe online if your computer breaks.

    Sharing: It gives you a web link so others can see and get your project.

## 3. Online Collaboration and Features 
Because your project is on GitHub's website (the cloud), it is easy for teams to work together.

Collaborate: People around the world can see and suggest changes to your code.

Review Code: Team members can look at new changes before they are added to the main project.

Trace Issues: This means you can keep a list of bugs (problems) or new features that need to be fixed or added. It helps keep the project organized.


## What is a Repository?

A Repository (or Repo) is just the folder for your project.

Git watches and tracks everything inside this folder.

The folder holds:

    . Your code.

    . Notes and files (documentation).

    . The complete history of every change you've made.

Repos can live in two places:

    . Locally: On your own computer.

    . Remotely: Online (like on GitHub).


## 1. What is a Repository (Repo)? 
A repository is simply the main container for everything related to one specific project.

Think of it as a special project folder. It's special because it has a hidden Git structure inside it that keeps track of every file and every version change.

## 2. What's Inside? 
The repo holds everything needed for your project:

    . Code: The actual programs you write.

    . Documentation: Files that explain how the code works or how to use the project (like a "Read Me" file).

    . History: The most important part! It's the list of all your "commits" (saved versions), so you can always see the past and go back in time.

## 3. Local vs. Remote Storage 
    . Local Repo: This is the copy of the project that is right on your hard drive. You work on this copy every day.

    . Remote Repo: This is the copy that is online, usually on a service like GitHub. This is used for backup and for sharing with your team.

    . Analogy: The Local Repo is your messy desk at home where you do the work. The Remote Repo is the clean, organized filing cabinet at the office that everyone shares.




# git status
. **git status** is a Git command you type.
When you type **git status**, Git quickly looks at your entire project folder and checks to see if anything has changed since the last time you made a commit (your last save).

. It tells you the current state (status) of your project folder (repo).

. It answers the question: "What is different right now?"

. It shows:

    . If you have new files.

    . If you have changed files.

    . If files are ready to be saved (committed).

## What information does it give you?

| File Group | What it means | What Git says |
|----------|----------|----------|
| Untracked | These are new files that Git doesn't know about yet.| """Untracked files:""" |
| Modified | These are files you have changed since your last save (commit). | """Changes not staged for commit:""" |
| Staged | These are files you have chosen and marked as ready for the next save.| """Changes to be committed:""" |


## The Big Picture
The **git status** command is your control center. If you run it and see the message: "nothing to commit, working tree clean," it means your local work is perfectly matched to your last saved version!


# git config
. **git config** is the command you use to change how Git works.
1. What is Configuration?
Configuration is just a fancy word for settings. When you use git config, you are simply telling Git your preferences and details.
    . Think of it like: Opening the Settings menu on your phone or computer.
. It lets you set your personal preferences and information.
2. Why do I need to set my Name and Email?
Every time you make a commit (a save point), Git records who did the work. It uses your set name and email address for this.
    . This is important because when you share your project on GitHub, everyone can see who made which changes.
. The most important things you set are your Name and Email address. (Git puts this info on every save/commit).

|Level|Where it applies|The option you use|
|----------|----------|----------|
|Global|All your Git projects (on your computer).|--global|
|Local|Only the project folder you are in right now.|Default (no option needed)|

3. What does --global mean? 
The --global part is very helpful because it tells Git, "Use this setting for every Git project I ever work on."
    . If you don't use --global, the setting is only saved for the current project you are in. This is called local configuration.

Common Examples

    . Set your Name: git config --global user.name "Your Name"
    . Set your Email: git config --global user.email "your.email@example.com"
    . See all settings: git config --list


# git init

. **git init** is the first command you run in a new project folder.
. It initializes (starts) the Git tracking system.
. When you run it, it creates a hidden folder called **.git** inside your project folder.
. This **.git** folder is the "time machine" storage—it holds all the history, versions, and configuration.
. After **git init**, your folder becomes a local repository (a Git project).


## 1. What does it do?
The **git init** command is what turns a regular, boring folder on your computer into a special Git project folder (a local repository).
    . Think of it like: Pressing the "Start Tracking" button for a project.

## 2. The **.git** Folder (The Magic Box) 
When you run **git init**, Git creates a small, hidden folder named .git. This is the most important part!
    . This .git folder is where Git keeps all the necessary information to track changes—the entire history of your work is stored here.
   . If you accidentally delete this .git folder, your project is still there, but Git will forget all the history you saved!

### 3. How to use it:
    1. Create a new folder for your project (e.g., named "MyWebsite").
    2. Open your command line/terminal inside that folder.
    3. Type git init.

Result: Your project folder is now ready to use Git commands like git status, git add, and git commit.
