---

description: Initial description.

author: "@Luigi"
---

- git status, git add, git commit -m, git push, git clone repo
- New branch: git checkout -b my_branch
- git branch displays the branch you are in
- Once branch is created if you try git push it will say there's no upstream branch, so you have to created in the remote github repo with
	- git push --set-upstream origin my_new_branch
- Trying to understand git reset and git reset --hard (dangerous)
- Need to learn git rebase.
	- git checkout master, add some changes
	- git checkout feature and changes not there so
		- git rebase master will add the latest master changes and keeping the feature branch as it is
		- So is like pulling from master ¿?