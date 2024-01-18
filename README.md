# github-3.2-jody
Assignment 3.2

## Git Commands
#### Create repositories 
When starting out with a new repository, you only need to do it once; either locally, then push to GitHub, or by cloning an existing repository.  
 
```
git init - Turn an existing directory into a git repository

git clone [url] - Download a repository that already exists on GitHub, including all branches, commits and files
```

#### Branches
Branches are an important part of working with Git. Any commits you make will be made on the branch you're currently “checked out” to. Use git status to see which branch that is.

```
git status - See the differences between current file and index files

git branch [branch-name] - Creates a new branch

git branch -d [branch-name] Deletes the specified branch

git checkout [branch-name] - Switches to the specified branch and updates the working directory|

git merge [branch] - Combines the specified branch’s history into the current branch. This is usually done in pull requests, but is an important Git operation.

```

#### Synchronize changes
Synchronize your local repository with the remote repository on GitHub.com

```
git fetch - Downloads all history from the remote tracking branches

git merge - Combines remote tracking branch into current local branch

git push - Uploads all local branch commits to GitHub

git pull - Updates your current local working branch with all new commits from the corresponding remote branch on GitHub.

```

#### Make changes
Browse and inspect the evolution of project files

```
git log - Lists version history for the current branch

git log --follow [file] - Lists version history for a file, including renames

git log branchB.. branchA - Show the commits on branch A that are not on branch B

git show [commit] - Outputs metadata and content changes of the specified commit

git add [file] - Snapshots the file in preparation for versioning

git commit -m "[descriptive message]" - Records file snapshots permanently in version history

git diff branchB..branchA - show the diff of what is in branchA that is not in branchB
```

#### Redo commits
Erase mistakes and craft replacement history

```
git reset [commit]<br><br>Undoes all commits after [commit], preserving changes locally

git reset --hard [commit]<br><br>Discards all history and changes back to the specified commit

git rebase [branch] - Apply any commits of current branch ahead of specified one

git rm [file] - Delete the file from project and stage the removal for commit

git mv [existing path] [new path] - change an existing file path and stage the move 
```

> [!caution]
> Changing history can have nasty side effects. If you need to change commits that exist on GitHub, proceed with caution.

---

## 4 commands that will be most used in a project

#### git add
We will always have to stage our commits before committing 
#### git commit -m "message"
We will always have to commit the staged material into a snapshot
#### git push
we will have to update the remote repository branch with our local branch commits 
#### git pull 
We will have to fetch and merge commits from the tracked remote branch to our local repository after teammates made their changes 

---

## GitHub Authentication 
To keep your account secure, you must authenticate before you can access certain resources on GitHub. When you authenticate to GitHub, you supply or confirm credentials that are unique to you to prove that you are exactly who you declare to be.

#### You can access your resources in GitHub in a variety of ways: 
1. Browser,
2. GitHub Desktop 
3. Another desktop application, with the API
4. Command line. 
#### Each way of accessing GitHub supports different modes of authentication.
1. Username and password with two-factor authentication, or a passkey
2. Personal access token 
3.  SSH key
