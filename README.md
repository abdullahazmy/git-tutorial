# git-tutorial
Advanced Git Tutorial with Tips and Tricks for Branching

> [!IMPORTANT]
> To contribute, Fork this repository, create a new branch from the main branch, make your changes, and submit a pull request. Include a description of your changes in the pull request description.

---

### Viewing the Commit Pointed by ‘HEAD’
To view the commit pointed by ‘HEAD’, you can use the following command:
``` bash
git show HEAD
```
This command will display detailed information about the commit, including the commit message, author, date, and the changes made in that commit. This can be useful when you want to review the most recent changes or understand the state of your repository.

#### a. Checking Out a Specific Commit

To move ‘HEAD’ to a specific commit, you can use the `git checkout` command followed by the commit hash or a branch name. For example, to move ‘HEAD’ to a commit with the hash ‘abc123’, you can run:
``` bash
git checkout abc123
```

If you don't know how to know the hash, you can use `git log --oneline` you can add any preferrations to it as you like, you can search about them with `git log -h` or 'man git log'

#### b. Moving ‘HEAD’ Relative to the Current Commit
You can also move ‘HEAD’ to a commit relative to the current commit using the `git checkout` command with the ~ or ^ notation. For example, to move ‘HEAD’ one commit back, you can run:
``` bash
git checkout HEAD~
```

Similarly, to move ‘HEAD’ two commits back, you can run:
``` bash
git checkout HEAD~2
```
This allows you to quickly navigate through the commit history and switch to a specific commit without specifying the commit hash or branch name explicitly.

---

### Creating a new branch at HEAD

Creating a new branch at the current commit pointed by ‘HEAD’ is a common operation, especially when you want to start working on a new feature or bug fix. To create a new branch at ‘HEAD’, you can use the following command:

```bash
git branch new-branch-name
```

This will create a new branch named ‘new-branch-name’ starting from the commit pointed by ‘HEAD’. You can then switch to the new branch using the git checkout command:

``` bash
git checkout new-branh-name
```

To push the current branch and set the remote as upstream, use

    git push --set-upstream origin branch-name
