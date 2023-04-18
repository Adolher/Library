# Windows Subsystem for Linux
## Installation

| command | short | description |
| --- | --- | --- |
| wsl --install |  | install WSL and default Ubuntu distribution |
| wsl --install --inbox |  | using the Windows component instead Microsoft Store (WSL updates will be received via Windows updates) |
| wsl --install --enable-wsl1 |  | enables WSL 1 during the install |
| wsl --install --no-distribution |  | do not install a distribution when installing WSL |
| wsl --install --distribution \<DistributionName> | -d | specify the Linux Distribution to install |
| wsl --install --no-launch | -n | do not launch the Distribution after install |
| wsl --install --web-download |  | install from an online source rather than from Microsoft Store |
| wsl --update |  | updates WSL |
| wsl --update --web-download |  | update from an online source rather than from Microsoft Store |
| wsl --update --pre-release |  | update to a pre-release ( if available ) |

## Some Settings

| command | short | description |
| --- | --- | --- |
| wsl --set-default \<DistributionName> | -s | set the default (standard) Distribution |
| wsl --set-default-version \<Version> |  | set the default WSL-Version |
| wsl --set-version \<DistributionName> \<WSL-VersionNumber> |  | set WSL-Version for the Distribution |
| wsl --import \<DistributionName> \<InstallationPath> \<FileName> |  | import the .tar-File with the specified Distribution at the specified Path |
| wsl --import \<DistributionName> \<InstallationPath> \<FileName> --version \<VersionNumber> |  | specifies a WSL-Version |
| wsl --import \<DistributionName> \<InstallationPath> \<FileName> --vhd |  | the Distribution-File is a .vhdx-File |
| wsl --export \<DistributionName> \<FileName> |  | export the Distribution as .tar-File |
| wsl --export \<DistributionName> \<FileName> --vhd |  | export the Distribution as .vhdx-File |
| wsl --import-in-place \<DistributionName> \<FileName> |  | import a .vhdx-File as a new Distribution (must be ext4) |

## Get Informations

| command | short | description |
| --- | --- | --- |
| wsl --help |  | show help |
| wsl --version | -v | show version of WSL |
| wsl --status |  | show status of WSL |
| wsl --release-notes |  | show WSL release notes in webbrowser |
| wsl --list | -l | lists installed Distributions |
| wsl -l --all |  | lists all Distribution, including those which are beeing installed and uninstalled |
| wsl -l --running |  | lists running Distributions |
| wsl -l --quiet | -q | show only names of Distributions |
| wsl -l --verbose | -v | show detailled information of all Distributions |
| wsl -l --online | -o | show available Distributions to install |

## Interact with a Distribution

| command | short | description |
| --- | --- | --- |
| wsl --user \<UserName> | -u | start Standard-Distribution as \<UserName> |
| wsl --distribution \<DistributionName> | -d | start \<DistributionName> |
| wsl --exec \<Command> | -e | run \<Command> without using Linux-Shell |
| wsl --shutdown |  | terminates all running Distributions and WSL |
| wsl --terminate \<DistributionName> |  | terminates the specified Distribution |
| wsl --unregister \<DistributionName> |  | Unregister ( Uninstall ) the Distribution |

## Mount / Unmount devices

| command | short | description |
| --- | --- | --- |
| GET-CimInstance -query "SELECT \* from Win32_DiskDrive" |  | Get available DeviceIDs in PowerShell |
| wsl --mount \<DeviceID> |  | mount a device in all WSL Distributions |
| wsl --mount \<DeviceID> --vhd |  | specifies that <DeviceID> refers to a virtual device |
| wsl --mount \<DeviceID> --bare |  | attach the Device but do not mount it |
| wsl --mount \<DeviceID> --name \<CustomName>|  | mount the Device with specified name |
| wsl --mount \<DeviceID> --partition \<PartitionNumber> |  | IndexNumber of the partition to mount |
| wsl --mount \<DeviceID> --type \<FileSystem> | -t | Filesystem to use when mouning the Device (default: ext4) |
| wsl --mount \<DeviceID> --options \<MountOptions> | -o | additionally filesystem-specific options |
| wsl --unmount \<DeviceID> |  | unmount the Device of all WSL Distributions |