# Git Simple Test and Tutorial
my git tutorial

## Git Basics - Tips and Tricks
https://git-scm.com/book/en/v1/Git-Basics-Tips-and-Tricks

## Example Auto completion setup on MAC
https://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion

## Reset all from your git directory and go back origin/master branch
git checkout master && git reset --hard HEAD && git clean -f && git pull origin HEAD

On Mac, You can place it in your env path

```
vim gitreset

#!/bin/bash
git checkout master && git reset --hard HEAD && git clean -f && git pull origin HEAD

:wq (save & quit)

sudo cp gitreset /usr/local/bin/
sudo chmod +x /usr/local/bin/gitreset

To Test :

```




