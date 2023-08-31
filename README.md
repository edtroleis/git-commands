# config

```
git config --global user.name "Eduardo Troleis"
git config --global user.email "edtroleis@gmail.com"
```

# .gitignore

- Ignore directory and subdirectories

```
**__pycache__
```

# git log

```
git log -5                            # 5 latest commits
git log --oneline
git log --oneline -2
git log --before="2023-08-27"
git log --after="2023-08-27"
git log --since="2 days ago"
git log --before="1 month ago"
git log --author="Eduardo"
```

# Back to time

```
git checkout <commit_id>
git checkout master
```

# Some commands

```bash
git mv file1 file2                                    # rename files
git rm file3                                          # remove files

git diff --staged                                     # compare files ready to be commited with files commited
git diff commit1..commit2                             # difference between commits

git commit --amend "new message"                      # add something to commit
git restore --staged Notes.md
git reset HEAD~                                       # undo last commit, but keep changes in working dir
git revert HEAD^                                      # reverse the last commit (create a new one)
git cherry-pick <commit id>                           # apply only specific commit from another branch into current branch

git stash                                             # save uncommitted changes away temporarily so you can come back later on them
git clean                                             # delete untracked files/folders
git stash save "message here..."                      # store all modified tracked files for later use
git stash list                                        # show stored messages
git stash pop                                         # get back saved files

git push origin main                                  # send local repo to remote server
git pull origin main                                  # download updates of remote repository on your machine
git fetch upstream main                               # update local copy without merging it

git tag v1.4                                          # create an annotated tag at this point in history
git tag                                               # list tags
git tag -d <tag>                                      # remove tag
git switch -c bugfix-1.0.0                            # checkout tag to branch

git describe --tags                                   # find out what version you are currently using based off tags
git archive --format=zip --output=v1.zip v1.4         # zip up a particular release

git clone https://github.com/<user>/<repo>.git        # clone a public github project locally
git init                                              # initialize empty folder as Git repo
git status                                            # check which files have changed since last commit and where they're located

git merge <branch_name>                               # merge branch_name with current branch
git merge upstream/main                               # merge two branches together
git rebase upstream/main                              # reapply commits from other branch onto yours

git checkout -- .                                     # restore all files modified
git checkout -- <filename>                            # restore <filename> modified
```

# Store https credential

```bash
git config credential.helper store
```
