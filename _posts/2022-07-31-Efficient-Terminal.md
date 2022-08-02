---
title: "Efficient-Terminal"
date: 2022-07-31
---

(pre) what is shell (a capture from bird's linux), what's the default shell come with ubuntu, what are the common shells most widely used today.

## Switch from bash(default shell) to zsh
 if cannot change the default shell by command line
 ```
 chsh -s $(which zsh)
 ```
 And it return 'user does not exist in /etc/passwd', you could use 'X-terminal-emulator', and configure a shell in 'Terminator Preferences' --> 'Profiles'-->'Command'--> Check 'Run a custom command instead of my shell'-->'Custom comand:/usr/bin/zsh' 

## Install zsh 

## Install and configure oh-my-zsh

## Install exa as replacement of ls 
Official site of [exa](https://the.exa.website/), as described in this [Issue](https://github.com/ogham/exa/issues/783), it's not available in Ubuntu 20.04 repository. But we could download the binary and install it manually.(Just put binary, manual and auto-completation setting file to correct path)
From above offical site download zip package, and it contain 3 folders for binary, manual, and auto-completation setting.


### Install download binary (where to put binary file, manual file, and config auto completion)

 - binary -->  /usr/bin
 - manual -->  /usr/share/man/man1 (or man2...5)
 - auto-complete setting for shell bash ---> /usr/share/bash-completion/completions
 - auto-complete setting for shell zsh ---> /usr/local/share/zsh/site-functions, and rename the file to '_exa'

