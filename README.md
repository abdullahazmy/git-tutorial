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

#### Checking Out a Specific Commit

To move ‘HEAD’ to a specific commit, you can use the `git checkout` command followed by the commit hash or a branch name. For example, to move ‘HEAD’ to a commit with the hash ‘abc123’, you can run:
``` bash
git checkout abc123
```
