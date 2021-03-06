# git-workflow
practise git workflow and commands

### Git rebase usage scenario
>>>>>>> fd4f9a73ae802cac89adb73eb365633e3b3b93da
1. Checkout `feature` branch from `master`.
2. Work on `feature` branch, and make commits.
3. Whilst there are new commits created on `master`
4. Use `git rebase` on `feature` branch, instead of merging `feature` with master and create redundant merge branch.
5. `git rebase --interactive <base>` Interactive mode lets clean up history by removing, splitting, and altering an existing series of commits.

### Delete last commit
1. `git rebase -i HEAD~2`, delete last line in editor.
2. `git reset --hard HEAD^`
3. Use `git push --force` to force update upstream.

### Edit last commit (add files to last commit)
1. <`git reset HEAD`>, then edit and add changes to the stage.
2. `git commit --amend --no-edit`

### Rewrite history with `git commit --amend`
1. `git commit --amend -m` Edit previous commit's message.

### Merge branch
1. `git merge --ff` or `git merge --no-ff`

### Git Cherry Pick
