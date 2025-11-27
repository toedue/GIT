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


### 1. What does it do?
The **git init** command is what turns a regular, boring folder on your computer into a special Git project folder (a local repository).

    . Think of it like: Pressing the "Start Tracking" button for a project.

### 2. The **.git** Folder (The Magic Box) 
When you run **git init**, Git creates a small, hidden folder named .git. This is the most important part!

    . This .git folder is where Git keeps all the necessary information to track changes—the entire history of your work is stored here.
    
   . If you accidentally delete this .git folder, your project is still there, but Git will forget all the history you saved!

### 3. How to use it:
    1. Create a new folder for your project (e.g., named "MyWebsite").
    2. Open your command line/terminal inside that folder.
    3. Type git init.

Result: Your project folder is now ready to use Git commands like git status, git add, and git commit.



# git branch
. A Branch is like a separate path or a parallel timeline for your work.

. It lets you work on a new feature or fix a bug without changing the main project code.

. The **git branch** command lets you see, create, and delete these paths.


### Common Uses of the Command:

|Command|What it Does|
|-----|---|
|git branch|Shows you all the branches you have. (The current one has a * next to it).|
|git branch <name>|Creates a brand-new branch with the name you give it.|
|git branch -d <name>|Deletes the branch you specify (after you are finished with it).|


###1. What is a Branch?
Imagine your main project code is a straight line on a road. When you create a branch, you are building a side road that splits off from the main one.

  . Main Branch (often called main or master): This road is for the safe, working, final version of your project.

  . Side Branch (e.g., new-feature-x): This side road is for all your new ideas, experiments, and fixes. If you break something here, the main road is still safe!

### 2. Why do we use Branches?
Branches are essential for two reasons:

  . Safety: You can write new code without the fear of messing up the code that everyone is using.

  . Teamwork: Different people can work on different features at the same time, each on their own safe branch.

### 3. The git branch Command
When you type git branch, Git shows you which roads exist and which road you are currently driving on (the one marked with the *).
  . It's like looking at a map to see all the different paths your project is taking.



# Initial Commit
. The Initial Commit is the very first save of your project's history in Git.

. It happens after you run the **git init** command.

. It starts the project's timeline.

. It usually includes a basic file or two (like a README file) to begin tracking.

. The message for this commit is often: "Initial commit".

## Making the First Save 
## 1. Why is it Special?
Every Git project needs a starting point, and the Initial Commit is that important starting flag.

Git Timeline: Imagine Git is building a long timeline of your project's life. The Initial Commit is Commit #1. All future commits (saves) will follow after this one.

Anchor Point: It acts as an anchor for your entire project's history. Without it, you can't really use Git's time-travel features.

## 2. The Simple Steps to an Initial Commit
You need three simple Git commands to make the Initial Commit happen:

    1. Preparation (git init): Turn your folder into a Git project.
    
    2. Staging (git add .): Tell Git, "I want to include all the files currently in this folder for the save."
    
    3. Saving (git commit -m "Initial commit"): Tell Git, "Okay, save everything I staged and write this message explaining what I did."

After these steps, your project has officially started its version-control journey!



# git add .
. git add is the command that tells Git you want to include files in the next save (commit).

. The dot (.) means "all the changes and new files in the current folder."

. This process is called Staging.

. Staging moves files from your working area to the Staging Area (a temporary holding place).

. You must git add before you can git commit.



## 1. What is the git add Command?
Think of your Git project having three main areas:

1. Working Area: This is your actual project folder where you are typing and changing files.

2. Staging Area: This is a holding box or a shopping cart for the next commit.

3. Repository (History): This is where your permanent saved versions (commits) live.

The git add command is the action of moving files from the Working Area into the Staging Area.

## 2. What does the . (Dot) Mean?
The dot (.) is a simple shortcut. In this command, it means: "Take all the new and changed files I have right now, and put them all in the Staging Area."

If you only wanted to stage one file, you would use its name instead: git add filename.txt. But using . is much faster for staging everything.

## 3. Why Stage?
Staging is important because it gives you control over exactly what you want to save.

. Imagine you made changes to ten files, but only six of them are completely finished and ready to be saved.

. You can use git add on those six files, leaving the other four unfinished ones in your Working Area.

. When you commit, Git only saves what is in your Staging Area (the six finished files).



# git commit

. **git commit** is the command that makes a permanent save of your project's progress.

. It takes everything in the Staging Area (what you prepared with git add) and locks it into history.

. -m stands for "message".

. The words inside the quotes (like "initial commit") are the explanation of what you changed in this save.


### The Full Process to Save:
    1. Stage (Select): git add . (Select all changes).
    
    2. Commit (Save): git commit -m "Your explanation" (Save the selected changes with a message).

## 1. What does git commit do?
This command is the final button press to create a snapshot (a copy) of your project at that moment in time.

. Before commit: Your changes are temporary.

. After commit: Your changes are permanently saved in the project's history (the .git folder). You can now safely "time-travel" back to this exact point if needed.

## 2. What is the -m and the Message?
Every save (commit) in Git needs a short note explaining what you did. This note is called the commit message.

. The -m tells Git, "The next thing I type is the message."

. Example message: "Initial commit"

    . This specific message is used for the very first save to show that the project is just starting its history.

. Example message: "Fixed bug on login page"

    . This message tells future developers (and your future self!) exactly why you made that save.


# `.git` Folder 

* It's a **hidden folder** that Git creates when you run `git init`.
* **What it does:** It holds **everything** that makes your project a Git repository.
* It contains all your project's **history**, all your **commits** (saves), all your **branches**, and all of Git's **settings**.
* It's the **"time machine" storage**. If you delete this folder, your project files remain, but **all of the history is lost**.
* **Rule:** **Never** manually change or delete files inside the `.git` folder! You must let Git manage it.



###  File States (Where is my file right now?)

* **File State:** Describes **where** a file is located in the Git process (e.g., is it saved? is it being worked on?).

### The Three Main States 

| State | Simple Explanation | What it Means | Command to Get Here |
| :--- | :--- | :--- | :--- |
| 1. **Modified** | **You changed it, but Git doesn't know you want to save it yet.** | The file is different from the last time you committed. This is your "working" area. | (Editing the file) |
| 2. **Staged** | **You prepared it for the next save.** | You told Git, "I want to save this file right now." It's in the temporary **Staging Area**. | `git add filename` or `git add .` |
| 3. **Committed** | **It's permanently saved.** | The file is safely stored as a **snapshot** in the `.git` history. | `git commit` |

### The Extra State

* **Untracked:** This is a **brand-new file** that has never been committed or told to be ignored by Git. It's totally new to the project. You must `git add` it first.

### How to Check the State

* You use the **`git status`** command to see which of the three main states all of your files are in.


# HEAD and Branching (Parallel Teamwork)

---

### 1. What is HEAD? 

* **HEAD** is Git's **pointer** to the **Commit** you are currently working on.
* It points to the **tip (latest save)** of the **current branch**.
* When you make a new commit, Git uses the location of **HEAD** to decide where to place that new save in the history timeline. It tells Git, "Start the new commit right here."
* **HEAD** = **Your current location** in the project's history.

---

### 2. How Branching Starts and Works

* **Creating a Branch:** When you create a new branch (e.g., using `git branch new-feature`), the new branch is just a **new pointer** that points to the exact same **Commit** as **HEAD** (your current location).
* **The Starting Point:** A new branch **always starts** from the Commit that the **HEAD** pointer is currently sitting on.
* **Parallel Work:**
    1.  You are on the `main` branch.
    2.  You create and switch to a new branch, `feature-A`.
    3.  Now, the `main` pointer and the `feature-A` pointer are separate.
    4.  Any new commits you make will only move the **`feature-A` pointer**, leaving the **`main` pointer** safe and unchanged.
    5.  This allows a teammate to work on `feature-B` on their own branch at the same time, without their changes affecting yours (or the main code) until the work is merged.

---

### 3. Why HEAD and Branching Enable Teamwork 

* **Safety (Isolation):** Branches keep new, risky, or unfinished work separate from the safe, working code on the `main` branch.
* **Parallelism:** Multiple developers can work on different tasks at the same time, each on their own branch, guaranteeing that one person's broken code won't stop the rest of the team.
* **Review:** When work is done, the team can review the changes on the branch before they are safely brought back into the main project's timeline (a process called **merging**).




# `git log` (Viewing History) 

* **Command:** `git log`
* **Show me the full history of my project saves (commits).**
* **What it Does:**
    * It prints a list of all the **commits** that have ever happened in the current branch's history.
    * It lets you look "backward in time" through your project.
* **What you see in the log:**
    1.  **Commit ID (SHA):** A long, unique number (like `c3b9b4f...`) that is the commit's fingerprint.
    2.  **HEAD/Branch Name:** Tells you where you and your branch pointers are.
    3.  **Author:** The name and email of the person who made the commit (`git config` info).
    4.  **Date:** When the commit was made.
    5.  **Commit Message:** The explanation you wrote using `-m "..."`.

### Useful Variations

| Command | Simple Explanation | What it Shows |
| :--- | :--- | :--- |
| `git log --oneline` | **Show me the quick version.** | Prints each commit on a single line (just the short ID and the message). |
| `git log -p` | **Show me the full changes.** | Prints the history **and** the exact lines of code that were added or removed in each commit. |




# `.gitignore` (The Exclusion List) 

* **What is it?** A plain text file named `.gitignore` that lists files or folders Git should **not track or save**.
* **A list of things Git should pretend don't exist.**
* **Why use it?**
    * To keep your project's history clean.
    * To prevent sharing large, unnecessary, or private files with your team or on GitHub.
* **What to Ignore:** You typically ignore files that are:
    1.  **Temporary:** Logs, cache files, etc.
    2.  **Private:** API keys or secret configuration files.
    3.  **Generated by the Computer:** Code compiled automatically (like `.exe` files) or downloaded files (like the `node_modules` folder in JavaScript projects).

### How to Use It

* You create a file named **`.gitignore`** in the root (top) folder of your project.
* You write the name of the file or folder you want to ignore on a new line.

| `.gitignore` Line | Simple Meaning |
| :--- | :--- |
| `temp.log` | Ignore the file named `temp.log`. |
| `*.exe` | Ignore ALL files that end with `.exe`. |
| `/node_modules` | Ignore the whole `node_modules` folder. |



# `.gitkeep` (The Empty Folder Trick) 

* **What is it?** A simple, empty file named **`.gitkeep`**.
* **A placeholder file used to force Git to track an otherwise empty folder.**
* **The Problem It Solves:**
    * Git is designed to **track files**, not folders.
    * If you create an empty folder in your project, Git **cannot save it** and will ignore it.
* **The Solution:**
    * You place the empty `.gitkeep` file inside the empty folder.
    * Now, the folder is **not empty**, so Git saves the folder (because it's saving the file inside it).
    * This ensures the empty folder structure is there when a teammate clones the project.
* **Note:** The name `.gitkeep` is just a **tradition**; it has no special meaning to Git itself. You could name the file `.placeholder` or `.keep` and it would work the same way.


---

# Branches

---
![Alt text](https://github.com/toedue/GIT/blob/main/branches.png)

### 1. What is a Branch?

* ** A Branch is just a lightweight, movable **pointer** to one specific **Commit** (a saved version).
* **Analogy:** Think of a branch as a **parallel timeline** or a side road that splits from the main road.
* Branches let you develop features, fix bugs, and experiment **without changing the main, stable code**.

### 2. Main Branches

* **`main` (or `master`):** This is the most important branch. It represents the **stable, working version** of your project.
* **`feature` Branches:** These are temporary branches created to hold new work (e.g., `feature/login-page`).

### 3. Parallel Work (Teamwork) 

* Branching is the **heart of Git teamwork** because it provides **isolation** (safety).
* **How it Works:** Multiple developers can work on different **feature branches** at the same time. Their changes are separate and safe until they are ready.
* This stops one person's broken code from affecting everyone else's stable work.

### 4. Ancestor and Inherited Commits

* **Ancestor Commit:** This is any **older commit** that came before the current commit in the history.
    * **Analogy:** Your ancestor commits are your grandparents and great-grandparents in the timeline.
* **Inherited:** When you create a new branch, it **inherits** (starts from) the history of the branch it split from. All those older commits are inherited by the new branch.

### 5. Merge and Merge Commit 

* **Merge:** The action of **combining** the changes from a separate branch back into the main branch.
    * Example: Taking all the code from your completed `feature/login-page` branch and bringing it into the `main` branch.
* **Merge Commit:** When you merge, Git often creates a **special new commit** called a **Merge Commit**.
    * This commit has **two ancestor commits** (the last commit on the feature branch AND the last commit on the main branch). It acts as a **record** showing that the two timelines were successfully joined.


# Creating and Switching Branches (Checkout vs. Switch) 

---

### 1. The Goal: Creating and Moving to a New Branch

The standard process to start working on a new feature safely is a two-step action:

1.  **First, make sure you are on the safe, stable branch** (usually `main` or `master`).
    * **Command:** `git switch main`
2.  **Second, create a new branch and move your HEAD pointer to it.**

---

### 2. The Old Command: `git checkout` 

* **Command:** `git checkout <branch-name>`
* ** A powerful, but **older** command used for many actions (moving between branches, undoing changes, restoring files).
* **Creating & Switching (Combined):**
    * `git checkout -b feature1`
    * **What it does:** The **`-b`** flag tells Git: "**b**uild a new branch named `feature1` **AND** immediately switch to it."

### 3. The New Command: `git switch` 

* **Command:** `git switch <branch-name>`
* A **newer** command introduced to be **safer and clearer** for only one job: **moving between branches.**
* **Creating & Switching (Combined):**
    * `git switch -c feature1`
    * **What it does:** The **`-c`** flag (for "**c**reate") tells Git: "**c**reate a new branch named `feature1` **AND** immediately switch to it."

---

### 4. The Difference Between `switch` and `checkout` 

| Feature | `git checkout` (Older) | `git switch` (Newer) |
| :--- | :--- | :--- |
| **Purpose** | **Multi-purpose** (used for switching branches, restoring files, and undoing history). | **Single-purpose** (only used for safely switching between branches). |
| **Safety** | **Less Safe:** Easy to accidentally overwrite or detach your HEAD pointer because it does too many things. | **Safer:** It prevents you from doing common mistakes related to accidentally losing work when switching. |
| **Best Practice** | Use mainly for **restoring files** (`git checkout -- <file>`). | Use for **all branch switching** (`git switch <branch>`). |

* The Git community created `git switch` and `git restore` (another new command) to split the many jobs of `git checkout` into clearer, safer commands. **For creating and moving branches, `git switch` is now the preferred method.**




# Git Merge 

---

### 1. What is Merge?

* Merge is the action of **combining** the history and changes from one branch (the source) into another branch (the target).
* **Goal:** To take finished work from a safe **feature branch** and update the stable **main branch** with those changes.

### 2. The Merging Steps

Before merging, you always follow a simple rule: **You merge FROM the finished branch INTO the branch you want to update.**

1.  **Go to the Target Branch:** First, you must switch your **HEAD** (your current location) to the branch that will *receive* the changes (usually `main`).
    * **Command:** `git switch main`
2.  **Run the Merge Command:** You then run the merge command, telling Git which branch to *bring in*.
    * **Command:** `git merge feature-branch-name`
    * **Result:** All changes from `feature-branch-name` are added to the `main` branch.

### 3. The Merge Commit

* A **Merge Commit** is a **special save** created when Git joins two timelines that have diverged (moved apart).
* Unlike a regular commit (which has one parent/ancestor), a Merge Commit has **two parents**—one from each of the branches being joined.
* It acts as a permanent record showing exactly *when* the two lines of development were brought back together.

### 4. Types of Merges 
![Alt text](https://github.com/toedue/GIT/blob/main/ff_merge.png)

Git handles merges in two primary ways, depending on the history of the branches:

| Type of Merge | Explanation | When it Happens | Result |
| :--- | :--- | :--- | :--- |
| **Fast-Forward Merge** | **Simple, straight-line merge.** | Happens when the target branch (`main`) has **not changed** since the feature branch split off. The history is still a straight line. | Git simply moves the target branch's pointer forward to the feature branch's latest commit. **No Merge Commit is created.** |
| **Non-Fast-Forward Merge** | **Creating a Merge Commit.** | Happens when **both branches have new commits** since they split. Their histories have diverged (moved apart). | Git must create a **Merge Commit** to formally join the two separate timelines and resolve any potential conflicts. |

![Alt text](https://github.com/toedue/GIT/blob/main/merges.png)





# Merge Conflicts 

---

### 1. What is a Merge Conflict?

* A merge conflict occurs when two branches being joined have **changed the exact same lines of code** in the same file.
* **Problem:** Git stops the merge because it doesn't know *which* change you want to keep. It asks for your **manual help** (resolution).
* **Result:** The file is marked with special conflict indicators (e.g., `<<<<<<<`, `=======`, `>>>>>>>`).

---

### 2. Resolving the Conflict (Choosing the Code)

When a conflict happens, you must manually edit the file to fix it:

1.  **Locate Markers:** Open the conflicted file and find the markers that separate the two versions:

    ```
    <<<<<<< HEAD (or your current branch, like 'main')
    This is the change on the branch you are currently on.
    =======
    This is the change on the branch you are merging from.
    >>>>>>> feature-branch-name
    ```

2.  **Choose the Code:** You must **delete the markers** (`<<<<<<<`, `=======`, `>>>>>>>`) and the code you *don't* want to keep.
    * **Choose the current branch's code.**
    * **Choose the incoming branch's code.**
    * **Choose both/Write New Code.** (Keep the parts you need from both sections and remove all markers).

3.  **Finish the Merge:** Once the file is clean (all markers are gone):
    * `git add <conflicted-file>` (Stage the file to show it's resolved).
    * `git commit` (This completes the merge, creating a merge commit).

---

### 3. Aborting the Merge (The Undo Button)

* **Command:** `git merge --abort`
* **Stop the entire merge process and go back to the state before you ran the `git merge` command.**
* **When to Use:** If you see too many complex conflicts and decide you need to fix the branches separately first, this command cleans up the mess and lets you restart.

---


![Alt text](https://github.com/toedue/GIT/blob/main/merge_conflict.avif)



# `git rebase`

---

### 1. What is Rebase?

*  Rebase is a way to **move** your branch to a different starting point. It **rewrites the project history** by moving your branch's commits and placing them one-by-one *after* the latest commit of the target branch.
* **Goal:** To keep the project's history **clean and linear** (a straight line) by avoiding the extra "Merge Commit" that a standard merge creates.
* **Warning:** Rebasing **rewrites history**. You should almost never rebase a branch that has already been pushed (shared) with others.

### 2. The Rebase Process

Imagine your `feature` branch split from `main` three commits ago, but `main` has two new commits since then.

1.  **Standard Merge:** Joins the two separate timelines and creates a special Merge Commit. (History is messy).
2.  **Rebase:**
    * Git **copies** your `feature` branch's commits.
    * Git **removes** the original commits.
    * Git **re-applies** your copied commits on top of the latest commit on `main`. (History is clean).

### 3. Rebase and Fast-Forward (FF) Merge 

* **The Result:** After you successfully rebase your `feature` branch onto `main`, the `feature` branch is now **ahead** of `main` by all of its commits. The timeline is now perfectly straight.
* **The Merge:** If you then run `git switch main` and `git merge feature-branch`, Git sees that the `main` branch can simply move its pointer forward to the `feature` branch's latest commit.
* Because the history is linear and `main` is an ancestor of the `feature` branch, the merge becomes a **Fast-Forward Merge**, and **no extra Merge Commit is created!**

**Steps to achieve a clean FF merge:**
1.  **Rebase:** `git switch feature-branch` then `git rebase main` (Moves `feature` on top of `main`).
2.  **Merge:** `git switch main` then `git merge feature-branch` (Performs a Fast-Forward merge).

![Alt text](https://github.com/toedue/GIT/blob/main/rebase.png)



# Git History Tools: `reflog` and `reset`

---

### 1. `git reflog` (The Safety Net/Journal) 

* **Command:** `git reflog`
* **A local journal of every single thing your HEAD has ever pointed to.**
* **What it is:** The **Reference Log** (`reflog`) tracks every time you moved or changed your **HEAD** pointer. This includes commits, checkouts, merges, and even rebases.
* **Why it's important:** If you accidentally use `git reset` or `git rebase` and think you've lost commits, the `git reflog` shows you exactly where your commits used to be, giving you a chance to **recover them**.
* The `reflog` only exists on your **local computer** and is your ultimate safety net for undoing mistakes.

---

### 2. `git reset` (The Undo Button) 

* **Command:** `git reset <commit-ID>`
* **To undo commits or unstage files by moving your branch pointer.**
* It moves your current branch pointer (and therefore your **HEAD** pointer) backward to a specific commit ID you choose.

### The Three Modes of `git reset` 

The `git reset` command is powerful because it works at three levels. The three flags determine how much it "undoes" in your project:

| Flag | Effect on **History** (Branch Pointer) | Effect on **Staged** Files | Effect on **Working** Files |
| :--- | :--- | :--- | :--- |
| **`--soft`** | Moves back to the target commit. | **Keeps** files staged. | **Keeps** files changed. |
| **`--mixed`** (Default) | Moves back to the target commit. | **Unstages** files. | **Keeps** files changed. |
| **`--hard`** | Moves back to the target commit. | **Unstages** files. | **DELETES** all local changes (use with extreme caution). |

### 3. Commit History

* The permanent, saved chain of snapshots (Commits) in the `.git` directory.
* **How to see it:** You view the commit history using the `git log` command.
* **Relationship to `reset`:** When you use `git reset`, you are not deleting the old commits from the history right away; you are just telling your **branch pointer** to ignore them. The old commits still exist and can be found using **`git reflog`**.

![Alt text](https://github.com/toedue/GIT/blob/main/reset.webp)




# `git diff` (Seeing Changes) 

* **Command:** `git diff`
* **Show me the line-by-line differences between two points in my project.**
* It compares two versions of your code and displays exactly which lines were **added** (shown with a `+`) and which lines were **removed** (shown with a `-`).

### Common Ways to Use `git diff`

The `git diff` command is used to compare files in the different stages of your project.

| Command | Comparison | Simple Question |
| :--- | :--- | :--- |
| `git diff` | **Working Area** vs. **Staging Area** | **"What changes did I make that I haven't added yet?"** (What is NOT staged?) |
| `git diff --staged` | **Staging Area** vs. **Last Commit** | **"What changes are ready to be saved?"** (What IS staged?) |
| `git diff HEAD` | **Working Area** vs. **Last Commit** | **"What have I changed in total since my last commit?"** |
| `git diff <branch1> <branch2>` | **Two Branches** | **"What's different between these two timelines?"** |

### Why it's Important

* **Review:** It lets you review your work before committing, acting as a final check to make sure you're not saving any unnecessary or accidental changes.
* **Debugging:** It helps you quickly pinpoint exactly what changed between two versions when you are tracking down a bug.



# `git cherry-pick` (Moving a Single Save) 🍒

---

### 1. What is Cherry-Pick?

* **Command:** `git cherry-pick <commit-ID>`
* **Take one specific commit (save) from one branch and apply its changes directly to another branch.**
* **Goal:** To transfer a single, small change (like a crucial bug fix) without bringing over all the other unfinished commits on the source branch.
* **Result:** Git copies the changes from the chosen commit and creates a **brand new commit** on your current branch. (The original commit remains where it was).

### 2. How to Cherry-Pick (The Steps)

1.  **Find the Commit ID:** Use `git log` or `git log --oneline` to find the unique ID (SHA) of the commit you want to copy.
2.  **Go to Target Branch:** Switch to the branch where you want the change to land (e.g., `main`).
    * `git switch main`
3.  **Cherry-Pick:** Run the command with the ID.
    * `git cherry-pick c3b9b4f`

### 3. Multiple Cherry-Picks and Maintaining Order

* **Multiple Commits:** You can cherry-pick multiple commits at once by listing their IDs in the order you want them applied.
    * `git cherry-pick <ID1> <ID2> <ID3>`
* **Maintaining Order:** Git will apply the commits **in the order you list them**. If the commits depend on each other (e.g., ID1 sets up the code that ID2 modifies), you must list them in the correct sequential order to avoid conflicts.
* **Conflicts:** Cherry-picking can cause **conflicts** if the changes in the single commit you're picking clash with the code on the target branch. You must resolve these conflicts manually, just like in a merge.

### 4. Cherry-Pick vs. Merge

| Action | `git cherry-pick` | `git merge` |
| :--- | :--- | :--- |
| **What is moved?** | **Only the single, chosen commit.** | **All commits** from one branch to another. |
| **History** | Creates a **new** commit ID. | Joins the timelines (often with a Merge Commit). |
| **Best For** | Moving one bug fix or hotfix. | Combining entire finished features. |

![Alt text](https://github.com/toedue/GIT/blob/main/cherry_pick.png)
![Alt text](https://github.com/toedue/GIT/blob/main/cherry_pick2.png)





# `git stash` (Temporary Storage)

---

### 1. What is Git Stash?

* **A temporary storage location** for unfinished work.
* **Goal:** To quickly save your current, uncommitted changes (both **Staged** and **Unstaged**) and clean up your **Working Area** so you can switch branches or handle an urgent fix without committing incomplete code.
* **Result:** The changes are saved in a **stash stack** (a list of temporary saves) and your files go back to the state of your last commit.

### 2. Adding Stashes (Saving Work)

| Command | Simple Explanation | What it Does |
| :--- | :--- | :--- |
| `git stash push` | **Save the changes and clear the folder.** | Saves all your modified files and your Staging Area, then resets your folder to the last commit. |
| `git stash push -m "Message"` | **Save with a message.** | Saves the work and lets you add a helpful name (message) so you can remember what the stash contains. |
| `git stash list` | **See all your saved stashes.** | Shows you the **stash stack**, listing each temporary save with an index (e.g., `stash@{0}`, `stash@{1}`). |

### 3. Stash Stack (The List of Saves)

* The **Stash Stack** is a simple **list** of all the temporary saves you've made.
* The most recent stash is always at the top, called **`stash@{0}`**. The one before that is **`stash@{1}`**, and so on.

### 4. Retrieving and Removing Stashes

| Command | Simple Explanation | What it Does |
| :--- | :--- | :--- |
| `git stash apply` | **Use the changes but keep the save.** | Takes the changes from the **most recent stash** (`stash@{0}`) and puts them back into your Working Area. The stash **remains** in the stack. |
| `git stash pop` | **Use the changes and delete the save.** | Takes the changes from the **most recent stash** (`stash@{0}`) and puts them back into your Working Area, and then **immediately removes** that stash from the stack. (This is most common). |
| `git stash apply stash@{N}` | **Use an older save.** | Applies the changes from a specific older stash (e.g., `stash@{2}`) and keeps the stash in the list. |
| `git stash drop` | **Delete the most recent save.** | **Removes** the most recent stash (`stash@{0}`) from the stack **without applying** its changes. |
| `git stash clear` | **Delete all saved stashes.** | **Removes every single stash** from the stack permanently. |

**In short:** Use **`pop`** when you're done with the save, and use **`apply`** if you think you might need the same changes later or on another branch.






# Remote Repositories and Synchronization (Push, Pull, Clone)

---

## 1. Setting Up the Connection (Local to Remote)

###  Key Terms

* **Remote:** The online copy of your repository, hosted on a platform like GitHub.
* **Origin:** The standard **alias (name)** Git gives to the URL of the primary remote repository you are connected to.
* **Local Repo:** The copy of the project on your machine.

### The Steps to Connect a New Local Repo to GitHub

1.  **Initialize Repo on GitHub:**
    * **Action:** Go to GitHub and create a new, empty repository. GitHub will provide you with a unique URL (e.g., `https://github.com/user/repo-name.git`).

2.  **Link Local to Remote:**
    * **Command:** `git remote add origin <URL>`
    * **Idea:** Tell your local Git repository: "I have an online remote copy, and I'm going to call it **origin**."

---

## 2. Getting a Remote Repo to Your Computer

###  `git clone` (Download the Entire Project)

* **Command:** `git clone <URL>`
* **SIdea:** **Download a remote project and set it up as a local repo.**
* **What it does:**
    1.  It downloads the entire project and its full history from the remote URL.
    2.  It automatically names the remote connection **`origin`**.
    3.  It automatically sets up the project folder with a local Git repository (`.git` folder).
* **Best Use:** This is the command you use when you want to start working on a project that someone else created online.

---

## 3. Sending and Receiving Changes

### `git push` (Sending Local Saves to Remote)

* **Command:** `git push <remote-name> <branch-name>`
* **Most Common Use:** `git push origin main`
* **Idea:** **Send your new local commits to the online remote repository.**
* **What it does:** It uploads all commits that are currently in your local branch's history, but are missing from the remote branch.
* **Initial Push (Setting Upstream):** The very first time you push a new branch, you must use the `-u` flag:
    * **Command:** `git push -u origin main`
    * **The `-u` flag** means "set upstream" and tells Git: "From now on, the `main` branch on my computer is connected to the `main` branch on **`origin`**." Future pushes can just be `git push`.

---

### `git pull` (Receiving Remote Changes)

* **Command:** `git pull <remote-name> <branch-name>`
* **Most Common Use:** `git pull origin main`
* **Idea:** **Download new commits from the remote and immediately combine them with your local branch.**
* **The `git pull` Shortcut:** `git pull` is actually a shortcut for two sequential commands: **`git fetch`** followed by **`git merge`**.

---

### `git fetch` vs. `git pull` (The Two Steps)

`git pull` combines two distinct actions:

1.  **`git fetch` (The Download):**
    * **Idea:** **Download the new history/commits from the remote, but DO NOT change your working files yet.**
    * **What it does:** It updates Git's knowledge of the remote repository. It lets you see what changes have happened online without messing up your local work.

2.  **`git merge` (The Combine):**
    * **Idea:** **Take the newly downloaded changes and combine them with your local branch.**
    * **What it does:** It updates your actual working files and your local commit history to match the changes that came from the remote.

* **Why use `fetch` alone?** You use `git fetch` when you want to see what changes are available online before deciding if you want to apply them (`merge`) or rebase your work.

---

## 4. Summary of Synchronization

| Command | Direction | Simple Purpose | Breakdown |
| :--- | :--- | :--- | :--- |
| **`git clone`** | Remote $\to$ Local | Get a project for the first time. | Downloads the whole repo and its history. |
| **`git push`** | Local $\to$ Remote | Share your new saves/commits online. | Uploads local commits to remote branch. |
| **`git pull`** | Remote $\to$ Local | Get the latest changes from the team. | **`fetch`** (download) $\implies$ **`merge`** (combine). |




