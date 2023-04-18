## tagging
|  | command | description |
| --- | --- | --- |
| - | git tag | lists all tags |
| - | git tag -l "v0.5.\*" | lists all tags with pattern "v0.5.\*" |
| - | git tag -a v1.0.0 -m "Version 1.0.0" | create an annotated tag with message |
| - | git tag v1.0.1 | create a lightweight tag |
| - | git tag -a v2.7 \<first digits of checksum> | tag a commit with checksum after committing |
| - | git tag -d v1.0.1 | delete the tag v1.0.1 |
