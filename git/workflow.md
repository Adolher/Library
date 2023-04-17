# git workflow basics
[see for detailed information](https://git-scm.com/book/de/v2)
___
## aliases
|  | command | description |
| --- | --- | --- |
| - | git config --global alias.\<alias> \<command> | creates the alias \<alias> for \<command> |
| - | git config --global alias.co checkout | creates the alias co for checkout |
| - | git config --global alias.last 'log -1 HEAD' | use -> git last
## configure git
|  | command | description |
| --- | --- | --- |
| - | git config --list --show-origin | shows settings from config --system / --global and --local |
| - | git config --global init.defaultBranch main | set the default branch-name to 'main' |
| - | git config --global core.editor "\<editor> | set default editor [commands](https://git-scm.com/book/de/v2/Anhang-C%3A-Git-Kommandos-Setup-und-Konfiguration#ch_core_editor)
| - | git config --global --edit | opens a user-specific configuration file |
| - | git config --local --edit | opens a repository-specific configuration file |
| - | git config --system --edit | opens a system-level configuration file |
| - | git config --global user.email "\<email-add> | save E-Mail-Address of current user |
| - | git config --global user.name "\<name> | save the name of the current user |
| - | git remote set-url origin \<remote-repository-link> | e.g. https://github.com/Adolher/test.git |
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

## inspect a repository
|  | command | description |
| --- | --- | --- |
| - | git log | shows information about repository history |
| - | git log --graph --format=reference --all | [see documentation](https://git-scm.com/docs/git-log#_commit_formatting) |
| - | git show \<commit> --stat | shows a summary of a commit |
| - | git remote -v | show remote repositories |

## tagging
|  | command | description |
| --- | --- | --- |
| - | git tag | lists all tags |
| - | git tag -l "v0.5.\*" | lists all tags with pattern "v0.5.\*" |
| - | git tag -a v1.0.0 -m "Version 1.0.0" | create an annotated tag with message |
| - | git show v0.5.1 | shows the tag data with tagged commit |
| - | git tag v1.0.1 | create a lightweight tag |
| - | git tag -a v2.7 \<first digits of checksum> | tag a commit with checksum after committing |
| - | git tag -d v1.0.1 | delete the tag v1.0.1 |

## .gitignore
|  | command / entry | description |
| --- | --- | --- |
| - | echo "\<filename> >> .gitignore | append \<filename> to .gitignore |
| - |  | [see documentation](https://git-scm.com/docs/gitignore)
| - | # comment | a comment |
| - | glob patterns | see [globster.xyz](https://globster.xyz/) | 
| - | *.txt | ignore all .txt files |
| - | !info.txt | but do track info.txt |
| - | /TODO | ignore TODO file in current dir, but not subdir/TODO |
| - | logs/ | ignore all files in any dir named 'logs' |
| - | logs/*.log | ignore 'logs/main.log' but not 'logs/sub/sub.log' |
| - | logs/**/*.log | ignore all .log files in 'logs' dir and all sub-dirs | 

## branch a repository
