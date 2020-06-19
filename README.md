# git-cheat-sheet
## git commands

`git status`

`git clone https://github.com/handypeter/git-cheat-sheet.git`

`git add`

`git commit -m "commited this text"`

`git branch newFeat1   // creates a new branch`
`git checkout newFeat1 // switches to the new branch`

or

`git checkout -b newFeat1 // creates and switches to the new branch in one step`

`git merge exampleBranch // merge exampleBranch to the current branch`

`git merge master // refreshing current branch with (last) master branch` 

`git branch -d exampleBranch // delete exampleBranch`

`git log // detailed list of commits`

`git log --pretty=format:"%h %s" --graph // oneline format with short hash and tree`

`git checkout oldHashVersion_onSameBranch  // HEAD pointer is still on most fresh version --> 'detached head'`

`git switch -c newThread // detached head position back in timeline, with opening a new timeline from this present`

`git revert HEAD // step back from last commit`
