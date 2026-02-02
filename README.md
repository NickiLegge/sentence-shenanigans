# sentence-shenanigans

## Terminal commands

### git flow

- Change to a new branch `git checkout BRANCH_NAME`
- Create branch from another branch `git checkout -b BRANCH_NAME` This will copy the code from the current branch but creahe a new one
- Stage a commit `git add *` (commit all changes) or `git add FILE_NAME` (commit single file). I normally do this step through the VS Code.
- Commit your code `git commit -m "this is a commit message"` The message should be a brief description of what was changed.
- Push your changes to github `git push origin BRANCH_NAME`
- Pull down the most recent changes in github `git pull origin BRANCH_NAME`

### working with directories

- Change directory `cd` 
- Change directory back `cd ../`
- Change directory to a specific folder `cd FOLDER_NAME`
- Put it all together! Move back two directories and then navigate into sentence-shenanigans from the desktop `cd ../../fun_stuff/sentence-shenanigans`
- make a directory `mkdir FOLDER_NAME`

### workflow steps for new feature development

- `git checkout develop` checkout the develop branch
- `git pull origin develop` pulls all code changes from github
- `git checkout -b new-branch-name` creates a new branch from develop
- after making changes, either stage from vs Code or use the commend `git add *`
- commit your changes with a comment `git commit -m "description of change"`
- push your changes to github `git push origin new-branch-name`
- This is when you would make a PR from your brabch to develeop
