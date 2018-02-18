add remote

git remote add origin [https://github.com/user/repo.git](https://github.com/user/repo.git)

or git@github.com:user/repo.git for ssh

git push --force --set-upstream origin master

**Worktree**

`git worktree add -b hotfix ../hotfix origin/master`

`cd ../hotfix`

commit changes

This would push directly to remote.

`git push origin HEAD:master`

or

`git push origin hotfix`

which would allow you to create a merge request

now you could delete hotfix

