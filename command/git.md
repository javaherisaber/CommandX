# Git

## revert changes made to your working copy
```bat
git checkout .
```

## revert changes made to the index (i.e., that you have added), do this. 
Warning this will reset all of your unpushed commits to master!
```bat
git reset
```

## revert a change that you have committed
```bat
git revert <commit 1> <commit 2>
```

## remove untracked files (e.g., new files, generated files)
```bat
git clean -f
```

## remove untracked directories (e.g., new or automatically generated directories)
```bat
git clean -fd
```