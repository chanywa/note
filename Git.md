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
