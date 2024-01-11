# github-3.1-jody
Assignment 3.1


## Create repositories 
When starting out with a new repository, you only need to do it once; either locally, then push to GitHub, or by cloning an existing repository.  
 
```
git init - Turn an existing directory into a git repository

git clone [url] - Download a repository that already exists on GitHub, including all branches, commits and files
```

## Branches
Branches are an important part of working with Git. Any commits you make will be made on the branch you're currently “checked out” to. Use git status to see which branch that is.

```
git status - See the differences between current file and index files

git branch [branch-name] - Creates a new branch

git checkout [branch-name] - Switches to the specified branch and updates the working directory|

git merge [branch] - Combines the specified branch’s history into the current branch. This is usually done in pull requests, but is an important Git operation.

git branch -d [branch-name] Deletes the specified branch
```

## Synchronize changes
Synchronize your local repository with the remote repository on GitHub.com

```
git fetch - Downloads all history from the remote tracking branches

git merge - Combines remote tracking branch into current local branch

git push - Uploads all local branch commits to GitHub

git pull - Updates your current local working branch with all new commits from the corresponding remote branch on GitHub.

```

## Make changes
Browse and inspect the evolution of project files

```
git log - Lists version history for the current branch

git log --follow [file] - Lists version history for a file, including renames

git show [commit] - Outputs metadata and content changes of the specified commit

git add [file] - Snapshots the file in preparation for versioning

git commit -m "[descriptive message]" - Records file snapshots permanently in version history
```

## Redo commits
Erase mistakes and craft replacement history

```
git reset [commit]<br><br>Undoes all commits after [commit], preserving changes locally

git reset --hard [commit]<br><br>Discards all history and changes back to the specified commit
```

 > [!caution]
> Changing history can have nasty side effects. If you need to change commits that exist on GitHub, proceed with caution.
