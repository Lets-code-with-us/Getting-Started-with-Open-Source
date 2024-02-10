# GITHUB

This blog is all about getting started with GitHub. It is associated with Let’s Code organization. Author is Dhruva Bhat S N. Let's see what all things are covered in this Blog:

1. [Creating Account](#creating-account)
2. [Creating a README](#creating-a-readme)
3. [Creating your First Repository](#creating-your-first-repository)
4. [Installation of Git](#installation-of-git)
5. [Git Commands](#git-commands)
6. [Source control with Git in Visual Studio Code](#source-control-with-git-in-visual-studio-code)
7. [Exploring GitHub Repository](#exploring-github-repositories)
8. [Fork a Repository](#fork-a-repository)
9. [Creating a Pull Request](#creating-a-pull-request)
10. [Codespaces](#codespaces)

Let’s explore each section.

## Creating Account:

Creating an account on GitHub is easier thing. Follow the steps according to below.

1. Go to the following website: [GitHub](https://github.com/)
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/adeefb0c-e647-477d-abc0-d5f16ee421d5)
2. Click on Sign Up
3. Enter your email id
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/43d89738-a8fa-4a79-a810-7f5ca58fecd2)
4. Create a strong Password
5. Add a username
6. Solve the puzzle to verify that you are human
7. Click on Create account
8. Enter the code received on registered email
9. 🎉Congratulation! You just created your GitHub account.

## Creating a README

Before creating the README.md file let’s see 👀 what is README.md README is file which tells us about the repository. It is similar to docs of a application where you will get to know how to use the application for what this application is used etc. in the same way a README file tells about repository. Wait!!!! Now what is Repository Repository is like a folder in your system which contains different files. In the same way repository contains files on cloud. Now Let’s see how to create a README.md file Steps to create a README file

1. As soon as you create your account it will redirect you to explore page of GitHub
2. In that explore page you will find two options one is of creating a repository and creating a README.
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/e70ab9cb-c588-4ccd-8544-e114c090924c)
3. Click on **Create** README file
4. Basically, now you are creating your GitHub profile. Its like how you create your social media about. It will show as “username/username is a special repository: its README.md will appear on your profile!”
5. Here first username refers to your username. Second username refers to a repository which contains your username as repository name.
6. The GitHub provides you a default Readme idea where you can design
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/089fdc21-8765-443b-9382-acc8530b8de5)
7. You can add all your details. Social links also you can add
8. You can explore some amazing GitHub profiles [here](https://github.com/matiassingers/awesome-readme)

## Creating Your First Repository

Let’s see how to create a repository!

1. In the home page you fill find a “+” symbol click on that
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/ea98b6cb-c4bf-4a61-83ab-2d5fa19f0d28)
2. Click on new Repository
3. Upon Clicking that you will get a page as below👇
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/e9f54852-072b-4b8d-9247-beb7148fd00b)
4. Provide a name for the repository.
5. Add a description to repository.
6. Choose whether you want to keep the repository private or public.
7. ✅ Check mark on “Add a README file”.
8. For now, we can create the repository. In the later section we can 👀 about “. gitignore” and “licence”.
9. Click on “Create repository”.
10. You just launched your first repository! 🚀
11. This is the initial look of your repository
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/a2735730-30b1-49d8-9a37-391a969aa8d2)
12. Later you can design the repository using markdown and you can add your files.

## Installation of Git

1. You can refer [Git Documentation](https://git-scm.com/doc)
2. Git for windows [here](https://git-scm.com/download/win)
3. Git for Linux [here](https://git-scm.com/download/linux)
4. Git for macOS users [here](https://git-scm.com/download/mac)

## Git Commands
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/8c8cdcfe-22a6-4f4d-bb48-71efda51ae3c)

### 1. SETUP
Configuring user information used across all local repositories.
- Set a name that is identifiable for credit when view
  ```bash 
      git config --global user.name “[first name last name]”
    ```
- Set an email address that will be associated with each history maker
  ```bash 
      git config --global user.email  “[valid-email]”
    ```
- Set automatic command line coloring for Git for easy reviewing 
  ```bash 
      git config --global colour.ui auto
    ```

### 2. SETUP & INIT 
Configuring user information, initializing and cloning repositories
- Initialize an existing directory as a Git repository
  ```bash
    git init
  ``` 
- Retrieve an entire repository from a hosted location via URL
  ```bash
    git clone [url]
  ```

### 3. STAGE & SNAPSHOT 
Working with snapshots and the Git staging area
- Show modified files in working directory. Staged for your next commit
  ```bash
  git status
  ```
- Add files as it looks now to your next commit (stage)
   ```bash
    git add [file]
   ```
- Unstage a file while retaining the changes in working directory
   ```bash
    git reset [file]  
   ``` 
- Diff of what is changed but not stored 
 ```bash
    git diff
  ```
- Diff of what is staged but not yet committed
 ```bash
  git diff --staged 
  ``` 
- Commit your staged content as a new commit snapshot
 ```bash
    git commit -m “[descriptive message]”
  ```

### 4. BRANCH & MERGE
Isolating work in branches, changing context, and integrating changes 
- List your branches.  A * will appear next to the currently active branch
 ```bash
  git branch
  ```
- Create a new branch at the current commit
 ```bash
  git branch [branch.name]
  ```
- Switch to another branch and check it out into your working directory
 ```bash
 git checkout
  ```
- Merge the specific branch’s history into the current one
 ```bash
  git merge [branch]
  ```
- Show all commits in the current branch’s history
 ```bash
  git log
  ```

### 5. INSPECT & COMPARE
Examining logs, diffs, and object information
- Show the commit history for the currently active branch
 ```bash
  git log 
  ``` 
- Show the commits on branch-A that are not on branch-B
 ```bash
  git log brachB. .branchA
  ```
- Show the commits that changed file, even across renames
 ```bash
  git log - -follow [file] 
  ```
- Show the diff of what is in branch-A that is not in branch-B
 ```bash
  git diff brachB…branchA
  ```
- Show any object in Git in human-readable format
 ```bash
  git show [SHA]
  ```

### 6. TRACKING PATH CHANGES
Versioning file removes and path changes
- Delete the file from project and stage the removal for commit
 ```bash
  git rm [file]
  ```
- Change an existing file path and stage the move
 ```bash
  git mv [existing-path] [new-path]
  ```
- Show all commit logs with an indication of any paths that moved
 ```bash
    git log - - start -M
  ```

### 7. IGNORING PATHS
Preventing non-orientational staging or committing of files
 
- Save a file with desired patterns as gitignore with either direct string matches or wildcard global
 ```bash
  logs/
*.notes
Patterns/
  ```
- System-wide ignores patterns for all local repositories
 ```bash
  git config - - global core.excludesfile [file]
  ``` 

### 8. SHARE AND UPDATE
Retrieving updates from another repository and updating local repos 
- Add a git URL as an alias
 ```bash
  git remote add [alias] [URL]
  ```
- Fetch down all branches from that Git remote
 ```bash
  git fetch [alias]
  ```
- Merge a remote branch into your current bring it up to date
 ```bash
  git merge [alias]/[brach]
  ```
- Transmit local branch commits to the remote repository branch
 ```bash
  git push [alias] [branch]
  ```
- Fetch and merge any commits from the tracking remote branch
 ```bash
  git pull
  ```

### 9. REWRITE HISTORY
Rewriting branches, updating commits, and clearing history
- Apply any commits of the current branch ahead of specified one
 ```bash
  git rebase [brach]
  ```
- Clear staging area, rewrite working tree from specified commit
 ```bash
  git reset - -hard [commit]
  ```

### 10. TEMPORARY COMMIT
Temporarily store modified, tracked files in order to change branches
- Save modified and staged changes
 ```bash
  git stash
  ```
- Write working from the top of stash stack
 ```bash
  git stash pop
  ```
- Discard the changes from the top of stash stack
 ```bash
  git stash drop
  ```



## Source Control with Git in Visual Studio Code

Now we will discover how to push code from Visual Studio Code (VS Code) to our GitHub account. Requirements

I. You must be logged in via GitHub on your VS Code

II. Git need to installed

Steps:
1. Open the project folder to your VS code workspace
2. Click on source control
3. In that you will get two options
   - Initialize repository
   - Publish to GitHub
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/400092db-7992-46cc-89d9-b9e8ba95ba4a)
4. Click on initialize repository.
5. Upon clicking you will get a screen as below
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/d1825f66-3db2-4a4d-8f39-86eedd6ce2fb)
6. Click on commit
7.	As soon as you click on commit it will ask for the commit message 
8.	Provide the committing message 
9.	After that click on the ✅ mark on right top of vs code editor
 ![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/7557a37f-0a6b-4d5d-8d61-dfc80bcfaa77)
10.	Click on publish branch 
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/acbf36e8-c7c7-49f1-8f31-e1485126cd17)
11. 11.	As soon as you click on Publish Branch it will pop a small window and it will ask whether you want your repository public or private. Choose as per your wish.
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/36f731cb-989d-45c2-b2ba-dde85d4ab37c)
12. 12.	As soon as you choose your repository will be published on your GitHub

        
## Exploring GitHub Repositories

Exploring GitHub repository is the best part of GitHub. In this section you can see your top repositories on the left side of the window. Below that you can see your recent activity like raised issues or pull request. In the middle of the window, you can see the works done by the persons you are following. On the right side of the window, **Latest Changes** will be there in that the changes done on GitHub will be there. Below that Explore Repositories will be there. Imagine that you want to work on a **Weather App** with tech stack **React**. Go to the search tab and then search as “Weather app” for your search also there is an option for filter where you can see different filter options. Working on the project we will check on the upcoming chapters.

## Fork a Repository

Fork means creating a personal copy of an existing repository. You will fork a repository when you want to work on an open-source project or if you want to experiment with your knowledge on the existing project and check the results. Let’s see how to fork a repository

Steps:

1. Search the repository of your wish
2. Click on the fork button
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/5f7076d5-0a18-4e72-843a-6b14473a489b)
3. If you want to change the name of the repository you can change according to your wish. Click on Create fork 
![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/fe74f0bc-0728-4377-b22a-801af1b8f533)
4. As soon as you click you will get the same repository on your GitHub profile.

![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/fa919503-a440-4e30-b9d8-5ba2227d84cf)

5. For contributing you need to check on issues that are currently available on the project. Else you can raise a new issue or with the tag “bug” if it is a problem or “enhancement” tag for adding a new feature.
6. Inside the issue comment that you are ready to work on the issues and if it is asked to explain the procedure you are following to solve the issues.
7. Wait for the owner to assign the issue to you
8. Once the issue is assigned to you, you can start work on it.

## Creating a Pull Request

When you contribute to an open-source project or you are updating an existing project you will do the changes in a new branch. After making the changes you need to create the pull request. Later it will be reviewed by the repository owner and it will be merged.

## Codespaces

Codespaces is a secured configurable, and dedicated development environment that works how and where you want it to. Let’s see how to create a Codespaces

Steps:

1. Click on Code
2. There you will have two choices
   - Local
   - Codespaces
3. Choose Codespaces

![image](https://github.com/dhruvabhat24/GitHub/assets/122305929/ed2a0c10-85e5-4c89-900d-75081df817d8)

4. In Codespaces click on Create Codespaces on the main When you click on Create Codespaces on the main branch and it will ask whether you want it in the web environment or desktop environment. If you choose the desktop environment it will open the repository files in the VS Code editor. Codespaces need uninterrupted internet connectivity. There are different setup procedures for different tech-based projects. You can check them on the official docs [here](https://docs.github.com/en/codespaces/guides)
5. Important note: The Repository files will not be stored in your system. Local stores the repository files on your system. No need for internet connectivity to work purpose. But if you want to push the code then you need internet connectivity.

# Written By 
- [Dhruva BhatS N ](https://github.com/dhruvabhat24)
- [Connect me on LinkedIn](https://www.linkedin.com/in/dhruvabhatsn/)
