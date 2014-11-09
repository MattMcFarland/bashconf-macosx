bashconf
========
A custom and modular .profile / .bashrc file

## Overview

A clean way to manage your .profile leveraging the `source` command.

## Rapid Install

`git clone https://github.com/MattMcFarland/bashconf.git $HOME`

## Review

Instead of putting any logic in .profile, simply use `source` to grab the `modules` you wish to add like so:
```bash
#
# Over-Engineered Bash Profile
# Optimized for Mac OS X
#



#
# Environment
# Special Bash environment settings (ulimit, memory, caching, etc)
#
#
source $HOME/.bashconf/.env



#
# Plugins
# Special plugin sources grouped here, safely added before path exports.
#
source $HOME/.bashconf/.plugins



#
# Path exports
# exporting paths, one way at a time.
#
source $HOME/.bashconf/.pathexports



#
# Custom Bash Functions / Alias
#
source $HOME/.bashconf/.func



#
# Bash Prompt Settings
#
source $HOME/.bashconf/.prompt
```
