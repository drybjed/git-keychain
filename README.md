# git-keychain

Script to manage SSH public keys in a git repository

## Installation

Put `git-keychain` somewhere in your $PATH.

## Security considerations

`git-keychain` has limited functionality when run from normal user account, because of system privileges (for example, normal users by default don't have access to other users' `~/.ssh/` directories). Because of that it was designed to be run with `root` privileges, either directly or by using `sudo`. Script does not invoke any privilege-elevated commands by itself. Special care was taken to make sure that `git-keychain` does only what it's supposed to do, but author does not take any responsibility for unintentional damage to services or systems on which the script is used.

## Basic usage

To see list of available commands, run `git keychain usage`. To see help about specific command, run `git keychain help <command>`.

