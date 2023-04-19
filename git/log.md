# git log

## inspect a repository
|  | command | description |
| --- | --- | --- |
| - | git log | shows information about repository history |
| - | git log --graph --format=reference --all | [see documentation](https://git-scm.com/docs/git-log#_commit_formatting) |

## Limiting The Output

| command | short | description |
| --- | --- | --- |
| --max-count=\<number> | -n \<number> <br> -\<number> | limit the output of \<number> commits |
| --since=\<date> <br> --after=\<date> |  | show commits made after specified date <br> example: --after="2023-04-19" |
| --until=\<date> <br> --before=\<date> |  | show commits older than specified date |
| --author=\<pattern> <br> --committer=\<pattern> |  | limits the output to commits whose authors/commiters matches the specified RegEx-pattern |
| --grep=\<pattern> |  | limits the output to commits whose log-message match the specified RegEx-pattern |
| --invert-grep=\<pattern> |  | limits the output to commits whose log-message do not match the specified RegEx-pattern |
| --merges |  | show only merge-commits |
| --no-merges |  | show only commits whose are no merge-commits |
