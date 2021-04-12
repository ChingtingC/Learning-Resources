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

### Get an existing Git repository

If you wanna use an existing repository instead of creating it by yourself, try to git clone!

`git clone git://XXXXX.git`

for example: `git clone git@github.com:ChingtingC/Learning-Resources.git`

### Make something change!

add a new file or update a file

`git add file_test_a.txt`

remove a file

`git rm file_test_b.txt`

leave a message about this change

`git commit`

### More

`git commit`
`git diff`
`git show`
`git status`
`git merge`
`git log`
`git reset`
`git restore`
`git revert`
`git stash`
`git fsck`
`git branch`
`git fetch`
`git pull`
`git format-patch`
`git am`
`git push`
`git remote add public-repo`
`git rebase`
`git switch`
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
