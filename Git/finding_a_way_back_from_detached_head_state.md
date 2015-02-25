## Finding a way back from 'detached HEAD' state

If you remember which branch was checked out before (e.g. `master`) you could simply

```
git checkout master
```

to get out of detached HEAD state.

Generally speaking: `git checkout <branchname>` will get you out of that.
