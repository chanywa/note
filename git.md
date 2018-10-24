## Revert
```
git reset --hard {commit-id}
git reset --soft HEAD@{1}
git commit -m "Revert to {commit-id}"
git push origin master --force
```

## Clean up forked git
```
git remote add upstream /url/to/original/repo
git fetch upstream
git checkout master
git reset --hard upstream/master
git push origin master --force
```

# Branch
## Rename
```
git branch -m old-name new-name
git push origin :old-name new-name
git push origin -u new-name
```

## Remove
```
git branch -D branch-name
git push origin :branch-name
```

## Clean up branches removed from the remote
```
git remote prune origin
```
