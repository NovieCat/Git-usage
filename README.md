# Git-usage

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| git init | initialize a local Git repository |
| git clone ssh or https | create a local copy of a remote repository |

### Basic Snapshooting

| Command | Description |
| ------- | ---------- |
| git status | check status|
| git add [filename]| add a file to the staging area |
| git commit -m "[message]" | commit changes |
| git rm -r [filename] | remove a file or folder |

<style>
table th:first-of-type {
    width: 100px;
}
</style>
### Branching & Merging

| Command | Description |
| --------| ----------|
| git branch | list all local branches(the asterisk denotes the current branch) |
| git branch -a | list all local and remote branches |
| git branch [branch name] | create a new local branch |
| git checkout [branch name] | switch to branch |
| git checkout -b [branch name] | create a new local branch and switch to it |
| git checkout -b [branch1] origin/[branch2] | clone a remote branch2 and switch to branch1(local branch1 tracks remote branch2) |
| git branch -d [branch name] | delete a local branch |
| git push origin --delete [branch name] | delete a remote branch |
| git merge [branch2] | if you are currently on branch1, then you will merge branch2 into branch1 |
| git fetch | fetch branches along with commits necessary to complete historys |
| git push | push changes to remote repository(if you have upstream branch and its name matches your current branch) |
| git push --set-upstream origin [branch2] | push the current branch and set the remote as upstream(current branch tracks remote branch2 from origin), can use -u to replace --set-upstream |
| git push origin HEAD:[branch2] | push current branch to upstream branch2 on the remote(branch2 does not match your current branch) |
| git push origin [branch name] | push current branch to the branch of the same name on the remote |
| git pull | update local reposiotory to the newest commit |
