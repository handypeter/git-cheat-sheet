# git-cheat-sheet
## git commands

`git status`

`git clone https://github.com/handypeter/git-cheat-sheet.git`

`git add modifiedFile.extension`

`git commit -m "commited this text"`

`git branch newFeat1   // creates a new branch`
`git checkout newFeat1 // switches to the new branch`

or

`git checkout -b newFeat1 // creates and switches to the new branch in one step`

`git merge exampleBranch // merge exampleBranch to the current branch`

`git merge master // refreshing current branch with (last) master branch` 

`git branch -D exampleBranch // delete exampleBranch`

`git log // detailed list of commits`

`git log --pretty=format:"%h %s" --graph // oneline format with short hash and tree`

- rename a local branch: `git branch -m oldName newName`

## walking back in time

### & deleting
- working directory (clean saved but not staged files): `git clean -fd`
- staged files (put back to working directory): `git reset HEAD -- .` 
- committed files (delete totally last commit changes): `git reset --hard HEAD~1`
- no delete, but a new(!) commit on timeline with the 1-step-back snapshot: `git revert HEAD`  step back from last commit

### only contemplating
- to a desired commit: `git checkout oldHashVersion_onSameBranch`  // HEAD pointer is still on most fresh version --> 'detached head'
-    a) jump out from contemplating the past: `git switch -`
-    b) or opening a new timeline from this present: `git switch -c newThread` // detached head position back in timeline
