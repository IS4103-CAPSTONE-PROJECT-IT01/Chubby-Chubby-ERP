# Chubby-Chubby-ERP
This is an ERP system for Chubby Chubby

Cheatsheet for how to edit md files: https://github.com/tchapi/markdown-cheatsheet/blob/master/README.md

## Project Management

We will aim to release every week. At the start of every week, a new branch will be created for that week for new features or changes to be committed. Concurrently a new Milestone will be created too. Once the release is done, the branch and the Milestone will be closed and another branch and Milestone will be created for that week. Milestones will be named as the versions of the project.

During the weekend before a week, Different items to be planned for that week's Milestone. This list of items will be updated as the week progresses. The items for a week include:
* Addition of new featres
* Enhancements to existing features
* Bugs in the existing code
Once an item has been resolved, mark it as Closed to track the progress of the Milestone.

## Contributing Procedure:
* Fork the team repo into your own GitHub account (Let's call it individual repo). If you have forked it, pull it at the start of every week to keep your repo updated.
* Clone your individual repo onto your desktop. When you want to update your individual repo with the latest changes fom the team repo, pull directly from the team repo into your LOCAL repo, then push from your LOCAL repo to your INDIVIDUAL repo on Git.
* Make your own branch on your individual repo if you wish. Preferably, each new feature should have its own branch.
  `git checkout -b <branch_name>`: this will check you out to the new branch
* Make your changes in the individual repo. In your changes, ensure:
  * Your code complies with CheckStyles rules
  * You have added JUnit tests for your new features
* Commit your changes to your local branch.
  * First, ensure that you are on the right branch, then use the following commands:
    To checkout to a particular branch, use `git checkout <branch_name>`
  * Once you are on the right branch, commit changes using the following commands:
    `git add .`: This will add all untracked files to your commit.
    `git commit -a -m "<MESSAGE_FOR_COMMIT>"`: Ensure that the message starts with a *VERB* in its infinitive form (e.g. Create, Update, Delete, Add)
* Once your changes are committed, push your local changes to your individual repo on Git.
  `git push origin <branch_name>`
* Make a pull request from your individual repo to the team repo. Ensure that the branch selected on your individual repo is the branch with the new changes, and the branch on the team repo the weekly branch (not the master branch).
* Your changes will go through Travis and Coveralls for Continuous Integration. Once done, the pull request is ready to be merged.
* Tech lead (I) will merge the green-checked pull requests to the team repo and the new changes will be on the team repo. However, such changes will remain on the weekly branch of the team repo till the end of the week when it will be merged to the master branch for release.
* Pull the weekly branch regularly to keep your local repo updated.
