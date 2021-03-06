# [Git](https://git-scm.com/)

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

## Open platform

1. [GitHub](https://github.com/)
    * [GitHub for Mobile](https://github.com/mobile)
    * [GUI with GitHub Desktop](https://desktop.github.com/)
    * [Command line with GitHub CLI](https://cli.github.com/)
    * Other features
        * [Codespaces](https://github.com/features/codespaces): connect development environment by browser or Visual Studio Code.
        * [GitHub Actions](https://github.com/features/actions): makes it easy to automate all your software workflows, now with world-class CI/CD.
        * [Secure at every step](https://github.com/features/security): ship secure applications within the GitHub flow.
        * [Code Review](https://github.com/features/code-review/)
        * [Project Management](https://github.com/features/project-management/)
        * [Integrations](https://github.com/features/integrations)
        * [Packages](https://github.com/features/packages)
2. [GitLab](https://about.gitlab.com/)

## Usage

### Need help!

If you have no ideas to do, just call help!

`git help`

### Set who you are :)

* method 1:

```
cat >> ~/.gitconfig <<\EOF
[user]
	name = Your Name on Git
	email = your-mail@yourdomain.com
EOF
```
* method 2:

```
git config --global user.name "Your Name on Git"
git config --global user.email your-mail@yourdomain.com
```

### Create a new repository

Wanna create a whole new repository!

```
mkdir git_repo_test
cd git_repo_test
git init
```

### HEAD, head & branch ... ?

* **branch** is a line of development. A single Git repository can track an arbitrary number of branches. Whenever you create a Git repository, a branch named **master** is created, and becomes the active branch.
* **head** is a named reference to the commit at the tip of a branch.
* **HEAD** means the current branch. It is a reference to one of the heads in the repository (except when using a detached HEAD).
* **detached HEAD**: Git allows you to check out an arbitrary commit that isn’t necessarily the tip of any particular branch. The HEAD in such a state is called "detached".

List all branches in the repository

`git branch`

Switch working directory to branch_A

`git switch branch_A`

Create and switch working directory to branch_B

`git branch branch_B`

Delete branch_C

`git branch -d branch_C`


### Get an existing Git repository

If you wanna use an existing repository instead of creating it by yourself, try to git clone!

`git clone git://XXXXX.git`

For example: `git clone git@github.com:ChingtingC/Learning-Resources.git`

### Make something change!

Add a new file or update a file:

`git add file_test_a.txt`

Remove a file:

`git rm file_test_b.txt`

Leave a message about this change:

`git commit`

### Share changes to public!

Use **git push \<repository\> \<refspec\>** to share your changes!

* **\<repository\>** means the "remote" repository that is destination of a push operation. This parameter can be either **a URL** (eg. `git@github.com:ChingtingC/Learning-Resources.git`) or **the name of a remote** (eg. `origin`).
* **\<refspec\>** specifies what destination ref to update with what source object. The format of a `<refspec>` parameter is `<src>:<dst>` or `<src>` (missing **:\<dst\>** means dst is the same as **\<src\>**). 
    * Example2: `branch_local:branch_remote` 
    * Example3: `branch_name`

Hence, you can share your changes!

`git push origin master`


### Show the working directory status!

`git status`

It may show 3 kinds of files:
1. Changes to be committed
2. Changes not staged for commit
3. Untracked files

In addition, there are also two kinds of files:
1. Committed
2. Ignored


## Git Concepts

### [The Object Database](https://git-scm.com/docs/user-manual#blob-object)

1. blob object: is nothing but a binary blob of data, used to store file data. It doesn’t refer to anything else or have attributes of any kind.
2. tree object
3. commit object
4. tag object

### More

`git diff`
`git show`
`git merge`
`git log`
`git reset`
`git restore`
`git revert`
`git stash`
`git fsck`
`git fetch`
`git pull`
`git format-patch`
`git am`
`git remote add public-repo`
`git rebase`
`git request-pull`
`git ls-tree`
`git count-objects`
`git repack`
`git prune`
`gitk`
`git hash-object`
`git submodule`
`git update-index`
`git write-tree`
`git read-tree`
`git checkout-index`
`git commit-tree`
`git cat-file`
`git merge-base`

ref: https://git-scm.com/docs/user-manual
