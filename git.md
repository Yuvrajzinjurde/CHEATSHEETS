VIDEO 1 (GIT)

- virsion controll system

- Developed by linux

- Basic introductions

VIDEO 2 (WORKING STAGING & REPOSITORY)

- Git Has Three States:

* Modified
* Staged
* Commited
* Stashed

VIDEO 3 (INSTALLATION)

- THERE ARE NO COMMANDS AS SUCH
  INSTALL BASED ON YOUR OS AND OTHER CONFIGURATIONS
  WITH DEFAULT SETTINGS.

VIDEO 4 (GIT CONFIGURATION, LEVELS)

    Local Configuration: Applies to a specific repository.

    	git config --local --list

    Global Configuration: Applies to the current user across all repositories.

    	git config --global --list

    System Configuration: Applies to all users on the system.

    	git config --system --list


    These settings are stored in the .git/config file within the repository directory.

VIDEO 5 (USERNAME AND EMAIL CONFIGURATION)

    To configure username and password.

    Local Configuration

    	git config --local user.name "Your Name"
    	git config --local user.email "your.email@example.com"

    Global Configuration

    	git config --global user.name "Your Name"
    	git config --global user.email "your.email@example.com"

    System Configuration

    	sudo git config --system user.name "Your Name"
    	sudo git config --system user.email "your.email@example.com"

    Command to check git version :

    	git --version

    To check Complete Git Config:

    	git config--list--show-origin

    To remove a specific setting for a specific level of config :

    	git config --global --unset user.name

    Remove the specific section

       	git config --global --remove-section user

    To view hidden folder ls

    	-a

VIDEO 6 (GIT HELP AND GIT STAUS)

    To get help for git cmds use

    	git help
    Or
    	git help init/commit

VIDEO 7 (GIT STAGES)

    Initialization of empty git repository

    	git init

    To check the status of the project

    	git status

    To add into staging area

    	git add <filename>
    Or
    	git add .(includes everything)

    To add into commited area

    	git commit -m "your message"

    To open file in linux opener

    	vi <filename>

    To check the number of commits

    	git log

VIDEO 8 (GIT DIFF COMMAND & TRACK CHANGES BETWEEN WORKING DIRECTORIES)

    To check difference between working area and staging area

    	git diff

    To check difference between staging area and repo area

    	git diff --staged

    To check difference between working area and repo area

    	git diff HEAD

VIDEO 9 (HOW GIT STORES DATA)

    To check the hash we use

    	git cat-file <commitID> -p

VIDEO 10 (RENAME AND RESTORE FILES IN GIT REPOSITORY)
To Rename a file
mv old_name new_name(does not move file to staging area)
git mv old_name new_name(move file to staging area automatically)
To revert changes from staging area
git restore --staged <fileName>
To revert changes
git restore <fileName>

VIDEO 11 (GIT BRANCHING )

    	to commit changes.

    		git commit

    	To create and switch to a new branch in Git in a single command.

    		git checkout -b new_branch_name

    	It is used to switch between branches or restore files in a Git repository.

    		git checkout existing_branch_name

VIDEO 12 (GIT BRANCHING)
To create and switch to new branch in single line

    	git checkout -b login_feature

    To switch branch

    	git checkout master

VIDEO 13 (RENAME OR DELETE BRANCH)

    To see all branches on local reposetory

    	git branch

    To create new branch

    	git branch new_branch_name


    To rename current branch

    	git branch -m <old name> <New name>

    To delete any branch  (Note You need to be on different branch than one your trying to delete)

    	git branch -d <Branch name>

    To delete any branch without mergin the changes

    	git branch -D <Branch name>

VIDEO 14 (GIT MERGE , MERGING TWO BRANCHES)

    To merge changes made on to different branches

    	git merge <Branch name>

VIDEO 15 (RESOLVE CONFLICTS WHILE MERGING TWO BRANCHES)

    Developer has two choose between the commit which one he/she wants to keep or both.

VIDEO 16 (GIT REBASE )
To merge changes from one branch into another by moving, combining, or modifying commits, resulting in a linear project history.
git rebase <Branch name>

VIDEO 17 (GIT REBASE)

    to create a commit ahead of the <branch name> with the current branch pointing to it.

    	git rebase <Branch name>

VIDEO 18 (INTERACTIVE REBASE)

    To use interactive rebase, allowing you to modify and rearrange commits interactively.

    	it rebase -i <Branch name>

VIDEO 19 (MODIFY OR CHANGE LAST COMMIT)
To modify the last Git commit by adding changes or updating the commit message.

    	git commit –amend

VIDEO 20 (GIT CHERRY-PIC)
To apply a specific commit from one branch to another, merging changes without merging the entire branch.
git cherry-pick commitID

VIDEO 21 (DETACHED HEAD GIT)
To move the HEAD to a particular commit

    	git checkout <commit id>

VIDEO 22 & 23 (GIT RESET)
To move branch from one commit to another

    	git reset <commit id> (–hard, –soft, –mixed)

VIDEO 24 & 25 (GIT STASH AND GIT STASHING )

    To switch branches without committing the current Branch, the stashed WD is saved in a ‘stash’ Area.

    	git stash

    To move : from ‘stash’ to WD

    	git stash pop

VIDEO 26 (DELETING AND CLEARING SHASHES)

    To bring back a particular stash to the WD

    	git stash apply <stash id>

    To delete a stash

    	git stash drop (<stash id>)

    To assign a stash a name

    	git stash save <stash name> :

    To list out all stashes

    	git stash list

    To delete all stashes

    	git stash clear

    creates a new branch with the stash data

    	Git stash branch <branch name>

VIDEO 27 (GIT CHECKOUT )
To checkout to the previous state
git checkout
to checkout to one commit back from the HEAD

    	git checkout HEAD~1

VIDEO 28 (GIT RESTORE AND SWITCH COMMAND)
To move to <new branch> (same as checkout but less powerful)
git switch <new branch>
To revert the changes (Used din case of any unintentional mistakes)
git restore

VIDEO 29 (GIT REVERT COMMAND)
to reverse a commit but this happens in a new commit (unlike reset which will completely remove a commit)

    	git revert (<commit id>)

VIDEO 30 (GITHUB INTRODUCTION)

    Github : SaaS which can host repos in the cloud

VIDEO 31 (WHY WE NEED GITHUB)

    Why GitHub?

    	Centralized Repository Hosting.
    	Collaboration Tools.
    	Visibility and Transparency:
    	Version Control
    	Community and Networking
    	Continuous Integration and Deployment (CI/CD):
    	Issue Tracking and Management
    	Documentation hosting
    	Integration ecosystem
    	Security features
    	COntributing to Open Source Projects

VIDEO 32 (GIT CLONE)

    To get the repo in the local along with its full history. For this, repo needs to be public.

    	git clone <HTTPS Url> -

VIDEO 33 (GITHUB SSH CONFIGURATION SETUP)
To identify oneself so that it doesn’t require entering a username and password every time.
SSH?
To use SSH, add the SSH key pair in the account settings.

VIDEO 34 (REPOSITORY CREATION)

    Creating a Repo in GitHub

    Option 1: Existing Remote Repo Create a connection between the remote and local repo. Next step is to push the code.

    Option 2: Start from scratch Create repo in GitHub Clone it, & do some work! Push changes

VIDEO 35 (ADDING OR RENAMING REMOTE )

    To create a connection between the remote and local repository.

    	git remote add <name> <URL>

    To rename the name of remote.

    	git remote rename <old-name> <new-name>

    To remove the remote connection.

    	git remote remove <name>

VIDEO 36 (PUSHING CHANGES INTO THE REMOTE REPOSITORY)

    To push the changes in the branch to the remote reposetory.

    	git push origin <branch-name>

VIDEO 37 (PUSHING LOCAL CHANGES INTO THE REMOTE REPOSITORY)

    To push the commits from the src branch to the target branch of the remote repo.

    	git push origin <src-branch-name>:<target-branch-name>

VIDEO 38 (GIT PUSH -U)

    To set the upstream of the local master branch. Later on only git push can be used.

    	git push -u origin <branch-name>

    	git push -u origin <src-branch-name>:<target-branch-name>

VIDEO 39 (DIFFERENCE BETWEEN MAIN AND MASTER)
Differences between the main and master branch.
There is no differemce as such these are just a names

VIDEO 40 (REMOTE TRACKING BRANCHES)

    main branch is default branch

    To create new file form terminal

    	touch <filename>

    To get the list of local branches

    	git branch

    To get the list of remote branches

    	git remote branch -r

VIDEO 41 (CHECKOUT THE REMOTE TRACKING)

    To switch to the remote branch

    	git checkout origin/branch-name

    it will create a local branch if not present and set up to track the remote branch of the same name.

    	git switch branch-name:

VIDEO 42 (GIT FETCH COMMAND)

    To get the changes or download the changes but not integrate with the working files just lets you see what others have been working on and merge them into your work directory.
    To see those changes then checkout to the origin main your local main branch won't be touched.

    	git fetch <remote><branchname>(git fetch origin main/master)

VIDEO 43 (GIT FETCH)

    	Git fetch

VIDEO 44 (GIT PULL COMMAND)
used to retrieve changes from remote repo but unlike fetch it actually updates our HEAD branch with the commits from the remote it is nothing but a combination of git fetch + git merge.
pull can result in Merge conflicts
git pull <remote><branchname>(git pull origin main/master)
The remote will default to the origin branch and will track whatever tracking connection is configured for the current branch.
git pull

VIDEO 45: (GIT PULL )

    	Git pull

VIDEO 46: (README.md FILE IN GITHUB)

    The readme file is like an entry point to learn about the project

    Md extension is markdown, which means it is a syntax for formatting text

VIDEO 47: (WHAT IS GIT HUB GIST)

    Git hub gists are simple ways to share code with others

    GitHub Gists are a way to share snippets or small pieces of code, notes,
    or any text-based information quickly and easily.

    	-	Code snippet sharing
    	-	Version control
    	-	Public or private sharing
    	-	Embeddable
    	-	Syntax highlighting
    	-	Forking and collaboration
    	-	Commenting
    	-	Revision history
    	-	API access
    	-	git.github.com

    We can create public or secret gist

VIDEO 48: (WHAT ARE GIT HUB PAGES)

    GitHub is a platform for hosting Git repositories and collaborating on software projects.

    	-	Repository hosting
    	-	Collaboration tools
    	-	Community engagement
    	-	Visibility
    	-	Integration ecosystem
    	-	Documentation hosting
    	-	Security features

VIDEO 49: (GIT HUB PAGES)
GitHub Pages is a feature of GitHub that allows users to
host static websites directly from their GitHub repositories :

    	-	Static website hosting
    	-	Free hosting
    	-	Custom domain support
    	-	Automated publishing
    	-	Jekyll integration
    	-	Version control
    	-	Project Pages
    	-	GitHub Actions integration



    CREATION OF GIT-HUB PAGES

    	-	Create a new repository or use an existing one.
    	-	Add HTML, CSS, and JavaScript files to the repository.
    	-	Enable GitHub Pages in repository settings.
    	-	Wait for the site to build.
    	-	Access your GitHub Pages site at https://<username>.github.io/<repository>.
    	-	Optionally, set up a custom domain by creating a CNAME file in the repository and configuring DNS settings with your domain registrar

VIDEO 50: (PULL REQUESTS)
What are pull requests?
They are not built-in features of git they are a part of GitHub, gitlab or gitbucket
What is its use?
They allow developers to allow team members to review the code
Allow approval and rejection of the work
PR are nothing but merging the branches

VIDEO 51 (RESOLVE CONFLICTS)

    to open file on linux viewer

    	vi <filename>

    to resole git conflict when we raise a pull requests

    pull the changes from main branch

    	git pull origin main

    then set up track to local branch main
    	git branch --track origin/main

    then pull changes if any

    then switch to another branch and merge it into the main with

    	git merge main

    now remove conflicts from file and then simply add and push it.

VIDEO 52 (ADD COLLABORATORS)

    How to add colaborators

    go to settings and add the collaborators by searching for the username of
    user.

    can add restrictions from setting to perticular bhranch to prevent

    the collaborator from doing things.

VIDEO 53 (GIT-HUB FORKING)

    Forking option on git HUB

    forking workflow enables anybody to try and make a contribution for
    repository.

    we can make our seperate copy of repo and make changes as we need.

    fork the repo  then clone th e forked repo and do your operations into it.

VIDEO 54. (GIT-HUB FORKING AND CLONE WORKFLOW)

    after making changes on the personal repo you can create pull request to
    the original repository

    it allows a project manager to accept contribution fron around the world without
    adding them  as actual owners.

    owner need to open pull requests.

VIDEO 55 (GIT TAGGING)

    Git tags

    by using git tag we can tag perticular commit so we can lable commits by refering tag

    we can goto perticular commit by using tags

    we can mark perticuar point with tags.

    Are used to mark versions

    there are two types of tags

    	-	1. lightweight tags - much like branch that doesn't change

    	-	2. annotated tags -  stores extra meta data including the author's name and emai, the
    		date and a tagging message like commit.

VIDEO 56 (SEMANTIC VERSIONING FOR SOFTWARE)
4.2.1
Semantic Versioning

    Semantic Versioning specs outlines a standardized Versioning system for a software releases.

    version consist of three numbers separated by .

    4 . 2 . 1
    major . minor . patch

VIDEO 57 (GIT TAG COMMAND)

    Tolists all the tags having *text* word

    	git tag -l "*text*"

    git view state of repo.this puts in detached head states

    git checkout <tag>

VIDEO 58 (CREATING TAGS)
To get the available tags

    	git tag

    To set the tag to some particular commit

    	git tag <tag>

    To point to particular commit using tag

    	git checkout <tag>

    To get difference between 2 tags

    	git diff v1.0.0 v1.0.1

VIDEO 61 (GIT REFLOG COMMAND)
keeps track of how we switched to branches, it shows only local logs

    	git reflog

VIDEO 62 (TRAVERSING THE REFLOG)
To shows logs of particular record from the nth commit
git reflog show branch_name@{n}

    git reflog show branch_name@{1.week.ago}

    can also take day\week\month based arguments

    	git diff branch_name branch_name@{n}

    used to see time based changes

VIDEO 63 (GET BACK LOST COMMITS)

    - git reflog can be used to get back lost commits

VIDEO 64 (CREATE GIT ALIASES)

    Setting up Alice's name and email globally

    	git config --global user.name "Alice"
    	git config --global user.email "alice@example.com"

    Setting up Alice's name and email locally (per repository)

    	git config user.name "Alice"
    	git config user.email "alice@example.com"

    Check Git Configuration for Alice:

    	git config --list --show-origin | grep alice

    View Repository Status

    	git status

VIDEO 65 (HEHEHEH WE ARE DONE WITH GIT 😃)

    END OF THE COURSE
