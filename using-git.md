git push --force --set-upstream origin master

**Worktree**

`git worktree add -b hotfix ../hotfix origin/master`

`cd ../hotfix`

commit changes

This would push to remote.

`git push origin HEAD:master`

or

`git push origin hotfix`

which would allow you to create a merge request

