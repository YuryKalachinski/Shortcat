# Shortcat for Git

## Shortcat for the pretty git log. Can be extended with the commit count parameter (lg -10, lg -35)
> git config --global alias.lg "git log --graph --all --oneline --decorate"

or

> git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"



## Shortcat for Sublime Text

1 Create a file named subl (or any name you'd like for the command to call for Sublime Text) without extension

2 Put this command inside the above file(Replace the path for executable if necessary):
> \#!/bin/sh <br/>
> "C:\Program Files\Sublime Text 2\sublime_text.exe" $1 &

3 Place that subl file inside the adequate command directory according to your OS and Sublime Text version (If you have doubts, check the above link comments section). In my case, I'm using Sublime Text 3 with Windows 10 64bit so I placed it in:
> C:\Program Files (x86)\Git\usr\bin

4 Now, in order for you to open the desired file, in git bash use (within file folder)
> subl filename