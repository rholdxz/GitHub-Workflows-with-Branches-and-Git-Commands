# GitHub Workflows with Branches and Git Commands

## How to connect GitHub into *`$BASH`*
### Step 1: Create a new local repo
1. Now let us create a new directory for our local repository.
   Create a ***`myrepo`*** directory by copying and pasting the ***`mkdir`*** command below into the terminal:
   
   ```bash
   mkdir myrepo
   ```
2. Go into the ***`myrepo`*** directory by copying and pasting the ***`cd`*** command below:
   
   ```bash
   cd myrepo
   ```
3. In this ***`myrepo`*** directory lets create a new local git repository using the ***`git init`*** command. Copy and paste the command below into the terminal:

   ```bash
   git init
   ```
4. A new local repository is now created, which you can verify by doing a directory listing by pasting the following command into the terminal window:
   ```bash
   ls -la .git
   ```
   
### Step 2: Create and Add a file to the local repo
1. Now lets create an empty file using the following ***`touch`*** command:
   ```bash
   touch newfile
   ```
2. Add this file to the repo using the following ***`git add`*** command:
   ```bash
   git add newfile
   ```
### Step 3: Commit changes
1. Before we can commit our changes, we need to tell git who we are. We can do this using the following commands (you can copy these commands as is, no need to enter your actual information):
   ```bash
   git config --global user.email "you@example.com"
   git config --global user.name "Your Name"
   ```
3. Once the repo has the ***`newfile`*** in it let’s commit our changes using the the following ***`git commit`*** command. Note that the commit requires a message which we include using the ***`-m`*** parameter:
   ```bash
   git commit -m "added newfile"
   ```
### Step 4: Create a branch
*Our previous commit created a default main branch called* ***`master`***.
1. To make subsequent changes in our repo, lets create a new branch in our local repostitory. Copy and paste the following ***`git branch`*** command into the terminal to create a branch called ***`my1stbranch`***:
   ```bash
   git branch my1stbranch
   ```
