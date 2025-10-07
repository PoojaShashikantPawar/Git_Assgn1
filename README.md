 Local Git Repository Initialization
Initialized local Git repository
Created initial.txt with initial content and committed to main branch
Demonstrated staging and unstaging operations:
Staged temp.txt and unstaged using git restore --staged temp.txt
Modified temp.txt, staged again, and unstaged using git reset HEAD temp.txt


2. Remote Repository Operations
Created remote repository on GitHub
Linked local repository to remote
Pushed initial commit to remote main branch
Modified initial.txt via GitHub web interface
Pulled changes using git pull origin main
Staged multiple files (file1.txt, file2.txt)
Unstaged file2.txt using git reset HEAD file2.txt
Committed and pushed file1.txt to remote
Documented working directory state using git status


4. Branching and Pull Request
Created g1 branch on remote repository via GitHub
Fetched and checked out g1 branch locally:
git fetch origin
git checkout g1
Added g1_file.txt on g1 branch
Committed and pushed to remote
Raised pull request from g1 to main
Successfully merged PR without conflicts
Pull Request Links:


PR #1: [g1 to main merge]
4. Local Git Operations
Get Updated Files
Executed git fetch origin and git merge origin/main
Ensured local main branch is synchronized
Reset Operations
Created commit with changes to initial.txt
Performed soft reset: git reset --soft HEAD~1
Used interactive staging: git add -p
Performed hard reset: git reset --hard HEAD~1
Demonstrated change loss using git status and git log
List Changes
Used git diff main g1 to show branch differences
Listed tracked and untracked files with git ls-files and git status
Create Local Branches
Created branch b1 from main, updated initial.txt
Created branch b2 from b1, added b2_file.txt
Created branch b3 from b2, modified b2_file.txt
On b3: staged multiple changes, used git reset --mixed HEAD to unstage
Selectively staged hunks using git add -p
Showed staged differences using git diff --staged


5. Branch Merging and Cleanup
Merge Operations
Merged b3 into b2
Merged b2 into b1
Merged b1 into main
Merge Conflict Resolution
Introduced merge conflict by modifying same line in initial.txt on b3 and b2
Resolved conflict manually during merge
Documented resolution process with screenshots
Branch Cleanup
Deleted local branches:
git branch -d b1
git branch -d b2
git branch -d b3
Deleted remote g1 branch:
git push origin --delete g1
6. Fork Operations
Forked repository to new repository under account
Made changes (added text to readme.md)
Created PR from forked repository to original repository's main branch
Fork PR Links:



7. Advanced Unstaging Challenge
Complex Staging Scenario
Modified initial.txt, b2_file.txt, and added challenge.txt
Staged all changes: git add .
Unstaged challenge.txt: git reset HEAD challenge.txt
Selectively staged lines in initial.txt using git add -p
Committed staged changes
Saved remaining changes: git stash
Popped stash: git stash pop
Resolved stash application conflict manually
Committed resolved changes
Remove and Revert Operations
Performed git rm operations on files
Used git revert to undo specific commits
Documented state after each operation using git status and git diff
Key Git Commands Used
# Repository Setup
git init
git remote add origin <url>
git push -u origin main

# Staging Operations
git add <file>
git add .
git add -p
git restore --staged <file>
git reset HEAD <file>
git reset --soft HEAD~1
git reset --mixed HEAD
git reset --hard HEAD~1

# Branch Operations
git branch <branch-name>
git checkout <branch-name>
git checkout -b <branch-name>
git merge <branch-name>
git branch -d <branch-name>

# Remote Operations
git fetch origin
git pull origin <branch>
git push origin <branch>
git push origin --delete <branch>

# Inspection Commands
git status
git log
git diff
git diff --staged
git diff <branch1> <branch2>
git ls-files



