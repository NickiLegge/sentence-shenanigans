# sentence-shenanigans

## Terminal commands

### Git flow

- Change to a new branch `git checkout BRANCH_NAME`
- Create branch from another branch `git checkout -b BRANCH_NAME` This will copy the code from the current branch but create a new one
- Stage a commit `git add *` (commit all changes) or `git add FILE_NAME` (commit single file). I normally do this step through the VS Code.
- Commit your code `git commit -m "this is a commit message"` The message should be a brief description of what was changed.
- Push your changes to github `git push origin BRANCH_NAME`
- Pull down the most recent changes in github `git pull origin BRANCH_NAME`

### Working with directories

- Change directory `cd` 
- Change directory back `cd ../`
- Change directory to a specific folder `cd FOLDER_NAME`
- Put it all together! Move back two directories and then navigate into sentence-shenanigans from the desktop `cd ../../fun_stuff/sentence-shenanigans`
- make a directory `mkdir FOLDER_NAME`

### Workflow steps for new feature development

- `git checkout develop` checkout the develop branch
- `git pull origin develop` pulls all code changes from github
- `git checkout -b new-branch-name` creates a new branch from develop
- after making changes, either stage from vs Code or use the commend `git add *`
- commit your changes with a comment `git commit -m "description of change"`
- push your changes to github `git push origin new-branch-name`
- This is when you would make a PR from your brabch to develeop

# Feature info
Mad libs style application that prompts users to provide different words to fill out a silly story.

This is a stand alone project meant for learning and fun! Huzzah!

## Requirements
Sentence Shenanigans should walk the user through filling out a mad lib style story by proving prompts for different categories of words. Once all prompts have been completed, the user should be presented with the completed story using their word selections.

- Present one word category at a time (e.g. provide 5 nouns)

- Next button at the bottom is disabled until all worlds are selected

- Once a category has enough words, the Next button will be enabled.

- Next button takes the user to the next prompt.

- Next button should change to Finish button if this is the last prompt

- There is a Back button at the bottom of prompts

- If this is the first prompt, the Back button is disabled

- Back button will to take the user to the previous prompt.

- If back button is selected all previously selected words should be remembered

- Progress bar or dots at the bottom should show level of completion

- Once all prompts are filled out and the finish button is clicked we will display a loader while the story is being constructed

- After showing the loader for ~1 second we will show the completed story

- All stories will have a title

- The page should have a top bar

- Top bar should include a button to start a new story

- Top bar should have a history drop down

- All stories for the current session should be stored

- History drop down should display a list of completed story titles that can be accessed

- Clicking a story title from the history drop down should load the story