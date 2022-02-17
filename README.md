# Git Command #

- **Ancestry**
```
1. Get parent commit of a commit: de1421f^/ HEAD^/master^/HEAD~1/git show HEAD^/git show HEAD~1
2. Get grant parent commit of a commit: de1421f^^/ HEAD^^/master^^/HEAD~2/git show HEAD^^/git show HEAD~2
```

- **Tree Listing**
```
1. List the contents of a tree object: git ls-tree HEAD
2. List the contents of a specific tree object: git ls-tree HEAD assets
3. Show the contents inside a tree: git ls-tree HEAD assets/
```
- **Filter and Log**
```
1. Filter last n log: git log -n
2. Filter last logs by since date: git log -since=2022-01-01
3. Filter last logs by until date: git log -until=2022-01-01
4. Filter last logs by days before git log -until=“3 days ago"
5. Filter log in a range of time: git log -after=2.weeks — bofore=3.days
6. Filter by author: git log —author=“Kevin”
7. Filter by keyword: git log —grep=“Initial”
8. Filter all from a commit to head: git log b447401938...HEAD
9. Any changes on a specific file: git log ViewController.swift
```
- **Format the commit log**
```
1. Show statistics about changes in a  commit: git log —stat
2. Format log: git log —formet=oneline/short/full/fuller/raw etc
3. Getting everything on online in the log: git log —oneline
4. Show graph of my commit: git log —graph
5. Show graph in a nice way: git log —graph —all —online —decorate
```
- **Branching basic**
```
1. List out all branches (Local and Remote): git branch -a
2. List out all local branches: git branch
3. List out all remote branches: git branch -r
4. Create a new branch: git branch branch_name
5. Know the head: cat .git/HEAD
6. List of file in head: ls -la .git/refs/heads/
7. Get the head commit of a branch: cat .git/refs/heads/master
8. Checkout branch: git checkout new_feature
9. Know status: git status
10. Add all changes to the staging area: git add .
11. Add a specific file to the staging area: git add file_name
12. Commit all: git commit -am “ABC”
13. Create and checkout branch: git checkout -b new_new_feature
```

- **Branch Comparison**
```
1. Compare two branches: git diff master..new_feature
2. Compare two branches in a short format: git diff —cooler-words master..new_feature
3. Compare two branches in the short format before the last commit of new_feature: git diff —cooler-words master..new_feature^
```

- **Branch merging**
```
1. Merge a branch to the current branch: git merge seo_title
2. Get the branch list which is merged with current: git branch —merged
3. Get the branch list that is not merged with current: git branch —no-merged
```

- **Rename and Delete**
```
1. Delete branch: git branch -d new_feature
2. Delete a branch that is not fully merged: git branch -D new_feature
3. Rename a branch: git branch -m new_feature seo_title 
```

- **Reset**
```
1. Soft Reset: Move commits in the staging area. Command: git reset —soft HEAD~1
2. Mix Reset: Move commits in unstaging area. Command: git reset —mixed HEAD~1/ git reset —HEAD~1
3. Hard Reset: Return to old state and discard all changes. Command: git reset —hard HEAD~1
```

- **Stash**: Pop and apply, both stashes make the file change but Pop delete stash but apply didn’t delete stash.

```
1. Stash save: git stash save “Change this”
2. View Stash: git stash list
3. Show a specific stash: git stash show stash@{0}
4. Show actual changes on a stash: git stash show -p stash@{0}
5. Retrieve stash: git stash pop
6. Retrieve a specific stash: git stash pop stash@{0}
7. Retrieve a specific stash by Apply: git stash apply 
8. Clear stash: git stash drop stash@{0} / git stash clear
```

- **Working with remote**
```
1. Push the branch to remote: git push -u origin master
2. Fetch remote changes: git fetch
3. Pull and merged: git pull  
4. Create branch from a remote branch: git branch non_tracking origin/non_tracking
5. Create and checkout branch from a remote branch: git checkout -b non_tracking origin/non_tracking
6. Push to remote using local branch: git push origin non_tracking
7. Push and delete the remote branch: git push origin:non_tracking/ git push origin —delete branch_name
8. Pushing to a remote branch: git push origin HEAD:refs/for/dev
```

# Xcode #
Show keyboard shortcut in xCode 

- Left bar menu open and hide:
```
command + 0 (zero)
```
- Left bar submenu open and hide:
```
command + (1/2/3/4/5/6)
```
- Right bar menu open and hide:
```
command + option + 0 (zero)
```
- Right bar submenu open and hide:
```
command + option + (1/2/3/4/5)
```
- Console / Debugger open and hide:
```
command + shift + y 
```
- Assistant Editor:
```
command + option + enter
```
- Search and Open a file:
```
command + shift + o
```
- Comment Multiple Line and undo comment:
```
command + /
```
- Format a block of code:
```
control + i
```
- Build a program:
```
command + b
```
- Run a program:
```
command + r
```
- Lookup a variable or method type: 
```
option + Click(left button of mouse or keypad) 
```
- Open a new file: 
```
 command + n
```



# Bash Command #
Most used command in bash MacOS

- Show all file in a directory as list:
```
ls
```
- Change directory:
```
cd
```
- Back to root directory:
```
cd ~
```
- Move one level down in a directory:
```
cd ..
```
- Move cursor to the first position of a sentence:
```
control + a
```
- Move cursor to the last position of a sentence:
```
control + e
```
- Clear the entire line:
```
control + u
```

- Make a folder in a directory:
```
mkdir folder_name
```
- Make a file in a directory:
```
touch filename_with_ext
```
- Open a file:
```
open filename_with_ext
```
- Open a file using an specific app: 
```
open -a appname filename_with_ext 
```
- Remove a file: 
```
 rm filename_with_ext
```
- Remove all file in a directory: 
```
 rm *
```
- Remove a directory: 
```
 rm -r directory_name/
```
