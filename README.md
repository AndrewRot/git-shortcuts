# git-shortcuts
A list of git shortcuts and commands

## Commandline shortcuts

.bash_profile aliases
```
alias gs='git status '
alias ga='git add '
alias gb='git branch '
alias gc='git commit'
alias gcm='git commit -m '
alias gd='git diff'
alias go='git checkout '
alias gk='gitk --all&'
alias gx='gitx --all'
alias gcem='git commit --allow-empty -m '
alias gri='git rebase -i '
alias grim='git rebase -i master '

gsquash(){
        git reset $(git merge-base master $(git rev-parse --abbrev-ref HEAD))
        git add -A
        git commit -m 'Squash to single commit'
}

```

.gitconfig settings

```
[push]
	default = current
[branch]
	autosetuprebase = always
```

