# git workflow basics
[see for detailed information](https://git-scm.com/book/de/v2)
___
## create and push a git repository
| step | command | description |
| --- | --- | --- |
| 0 | | move to projects directory or create one |
| 1 | git init |  |
| 2 | git add <filename(s)> | git add . -> git add all files in directory |
| 3 | git commit -m "initial commit" |  |
| 4 | git branch -M main | rename master-branch to main-branch |
| 5 | git remote add origin \<remote-repository-link> | e.g. https://github.com/Adolher/test.git |
| 6 | git push -u origin main |  |
___
## clone a repository
| step | command | description |
| --- | --- | --- |
| 0 | | move to directory where project should be in |
| 1 | git clone  \<remote-repository-link> | e.g. https://github.com/Adolher/test.git |
___
## work on a repository (single)
| step | command | description |
| --- | --- | --- |
| 0 | | move to projects directory |
| 1 | git pull | get the actual repository to working directory |
| (1-1) | git fetch | get the actual repository to staging area |
| (1-2) | git checkout | update files in working directory to match the staging area |
| 2 | | work on your project |
| - | git restore \<filename> | discard changes in working directory |
| (2.5) | git diff | show differences between working directory and staging area |
| 3 | git status | show which files are in which state |
| 4-1 | git add \<filename> | add \<filename> to staging area |
| - | git restore --staged \<filename> | unstage a file |
| 4-2 | git commit -m "\<message> | commit (move) changes to repository |
| (4) | git commit -a | commit changes by skipping the staging area |
| - | git commit --amend | replace the last commit |
| 6 | git push -u origin main | move changes to remote repository |
___
## branch a repository
