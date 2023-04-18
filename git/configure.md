# Configuring git

## aliases
|  | command | description |
| --- | --- | --- |
| - | git config --global alias.\<alias> \<command> | creates the alias \<alias> for \<command> |
| - | git config --global alias.co checkout | creates the alias co for checkout |
| - | git config --global alias.last 'log -1 HEAD' | use -> git last
___
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
___