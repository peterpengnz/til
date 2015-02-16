## Git and Aliases

I type `git status` or other git commands so many times a day.
So I want to save few minutes from my day and try to be DRY.

In `~/.bash_profile` file add following line and `source` it.

```
alias g="git"
```

Then execute following command in your console:

```
g config --global alias.co checkout
g config --global alias.ci commit
g config --global alias.st status
g config --global alias.br branch
g config --global alias.hist 'log --pretty=format:"%h %ad | %s%d [%an]" --graph --date=short'
```

Now you can type `g st` instead of `git status` :P
