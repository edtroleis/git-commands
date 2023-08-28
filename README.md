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

```
git mv file1 file2          # rename files
git rm file3                # remove files
git diff --staged           # compare files ready to be commited with files commited
git diff commit1..commit2   # difference between commits
```
