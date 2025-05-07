## GitHub repository link with merged branches ##
https://github.com/Sindhu3113/Git_GitHub_Medium_Assignment


## Screenshots of merge conflict and resolution process ##
![Conflict_img](conflicts.png)
The above img shows the merge conflict beacuse both the branches (add-content branch and master branch) make changes to the same lines in the same file(index.html), by which git cannot determine which change to keep, so git shows a merge conflict.

![conflict_resolved_img](conflicts_resolved.png)
I have resolved the merge conflict manually in GitHub by keeping the both changes and then committing the result.

![merge_successfull img](merge_successfull.png)
The merge conflict has resolved successfully 

## How merge conflict is resolved ##
The merge conflict had occured because add-content branch and master branch make changes to the same line in the same file i.e index.html,  by which git cannot determine which change to keep, so git shows a merge conflict. 
I resolved the conflict manually in GitHub by accepting both the changes, and then committed the changes(by clicking on commit changes) and after commiting the changes it displayed a UI to Merge Pull Requests(i.e there is no conflicts you can merge the branches).
After clicking on the merge Pull request both the branches got merged successfully.

## ASSIGNMENT 4 ##

## Git Hooks ##
Git hooks are scripts that run automatically when  certain events occur in Git WorkFlow, such as commit, merge and pull

staged changes->pre-commit->commit->pre-push->push->pre-recieve->repository

## common Hooks ##
1. pre-commit : runs before a commit is finalized 
2. commit-msg : runs after entering a commit msg
3. pre-push : runs before pushing code to a repository

git hooks are scripts stored in the .git/hooks directory of a Git repository.
hooks are stored in .git/hooks/
This directory contains sample hook scripts, such as
pre-commit.sample
commit-msg.sample
pre-push.sample

## Git Automation ## 

Git automation refers to using scripts, tools to automatically perform tasks during or after git operations. To improve consistency, code quality, Enforce code standards, Prevent bad commits or pushes.

## There are some Key Tools for Git Automation
1.Husky
2.lint-staged
3.ESLint

## Husky
Husky is a tool that makes it easy to set up and run Git hooks in your project directly.

## To install husky
npm install husky --save-dev

## To initialise husky pre-commit script
npx husky-init

it will create .husky/pre-commit file

## lint-staged

1. lint-staged runs linters only on files that are staged for commit.
2. lint-staged are used for faster commits because it checks only the staged files, cleaner code(automatically fixes lints and formats), prevents bad code from being commited

## installation and setup
## to install lint-staged
npm install --save--dev lint-staged husky

## working
1. if you stage files with git add .
2. lint-staged runs scripts only on those staged files, if the script passes, then commit proceeds else if the script fails, the commit is blocked.



