# Git Simple Test and Tutorial
my git tutorial

## Git Basics - Tips and Tricks
https://git-scm.com/book/en/v1/Git-Basics-Tips-and-Tricks

## Example Auto completion setup on MAC
https://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion

## Reset all from your git directory and go back origin/master branch
git checkout master && git reset --hard HEAD && git clean -f && git pull --all

On Mac, You can place it in your env path

```
vim gitreset

#!/bin/bash
git checkout master && git reset --hard HEAD && git clean -f && git pull --all

:wq (save & quit)

sudo cp gitreset /usr/local/bin/
sudo chmod +x /usr/local/bin/gitreset

Test Example :

thinegan@Thinegans-MacBook-Pro:~/mygit/gitest (test1) $gitreset 
Switched to branch 'master'
Your branch is up-to-date with 'origin/master'.
HEAD is now at 5509a5e shortcut
From github.com:thinegan/gitest
 * branch            HEAD       -> FETCH_HEAD
Already up-to-date.
thinegan@Thinegans-MacBook-Pro:~/mygit/gitest (master) $

```

## Intergrate Github with Trello
Example

### Git Branch Naming Convention :

1. Branch Type for grouping
bug       - Code changes linked to a known issue.
feature   - New feature.
hotfix    - Quick fixes to the codebase.

2. Format
{branch type}/{2-3 word summary}
Example :
feature/renderer-cookies
hotfix/dockerfile-base-image
bug/login-ie



```
Git set alias on frequently used command.
Eg. "git push origin HEAD"


Setup Alias :
git config --global alias.pu 'push origin HEAD'
Test : "git pu"   // git push origin HEAD

git commit -am "Set Alias"


Git set diff :
git config --global diff.tool vimdiff
git config --global difftool.prompt false
git config --global alias.d difftool
Test : "git d"    // git vimdiff

```

