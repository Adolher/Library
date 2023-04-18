# Windows Subsystem for Linux
## Installation

| command | short | description |
| --- | --- | --- |
| wsl --install |  | install WSL and default Ubuntu distribution |
| wsl --install --inbox |  | using the Windows component instead Microsoft Store (WSL updates will be received via Windows updates) |
| wsl --install --enable-wsl1 |  | enables WSL 1 during the install |
| wsl --install --no-distribution |  | do not install a distribution when installing WSL |
| wsl --install --distribution \<Distribution Name> | -d | specify the Linux Distribution to install |
| wsl --install --no-launch | -n | do not launch the Distribution after install |
| wsl --install --web-download |  | install from an online source rather than from Microsoft Store |

## Get Informations

| command | short | description |
| --- | --- | --- |
| wsl --list