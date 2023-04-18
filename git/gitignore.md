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
