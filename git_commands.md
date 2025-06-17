# Update local main
```
// From monorepo
git checkout master && git fetch upstream && git merge upstream/master && git push

// From polyrepo
git checkout master && git pull --rebase
```
# === git
alias g='git'
alias ga='git add'
alias gb='git branch'
alias gc='git commit -v'
alias gca='git commit -v --amend'
alias gcane='git commit --amend --no-edit' # make sure you git add {file} first
alias gpom='git push origin master'   #Bootcamp proj pilot
alias gpum='git pull upstream master' #Bootcamp proj pilot
alias gcob='git checkout -b'            # Create and switch to the new branch
alias gcm='git commit -m'
alias gco='git checkout'
alias gcoo='git checkout origin/master'
alias gcou='git checkout upstream/master'
alias gd='git diff HEAD'
alias gf='git fetch'
alias gfu='git fetch upstream'
alias gfa='git fetch --all' #Fetch all remote repos
alias gl='git log --stat'
# alias gll='git log --stat -p'
# alias gmc='git ls-files -u | cut -f 2 | sort -u' # show all files with merge markers
alias gr='git remote -v'
alias grb='git rebase'
alias grbum='git rebase -i upstream/master'
alias grbom='gco master && git pull --rebase && gco - && git rebase -i origin/master'
alias gcont='git rebase --continue'
alias gskip='git rebase --skip'
alias gabort='git rebase --abort'
alias gs='git status -sb'
alias gu='git unadd'                 # git config --global alias.unadd reset HEAD # https://tanzu.vmware.com/content/blog/git-unadd
alias updatemr='git checkout master && git fetch upstream && git merge upstream/master && git push'
alias updaterepo='git checkout master && git pull --rebase' # polyrepo workflow

# === git stash
alias gst='git stash'
alias gss='git stash save'
alias gsl='git stash list'
alias gsd='git stash drop' # git stash drop 9 remove the 9th stash
alias gsa='git stash apply'
alias gp='_git_push_auto_branch'     # git push to origin on current branch if no argument specified. Otherwise, git push to specified remote.
# alias glc='_git_commit_diff'         # show commit diff against upstream/master. Use origin if upstream doesn't exist
# alias glcc='_git_commit_all'         # show all commits
