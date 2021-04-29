## Implementing support for semantic versioning using only git aliases

[![image](https://user-images.githubusercontent.com/155492/116517998-0249ff80-a8d0-11eb-80b0-1018ab1a63a8.png)
](https://www.inc-inc.dk/stories/git-aliases)
**Click image to go the the full-length detailed blog on the implementation**


Original file is [`.gitconfig`](https://raw.githubusercontent.com/lakruzz/semver_git_alias/main/.gitconfig) in the [lakruzz/semver_git_alias](https://github.com/lakruzz/semver_git_alias) repo. Everything that goes on in this file is described in detail in my blog [__Git Aliases__](https://www.inc-inc.dk/stories/git-aliases).

# Install

Copy [`.gitconfig`](https://raw.githubusercontent.com/lakruzz/semver_git_alias/main/.gitconfig) from [this repo](https://github.com/lakruzz/semver_git_alias) to the root of your own repository, then CD into the repository and run:

```bash
git config --local include.path ./../.gitconfig
```

Hereafter all the git aliases will be availbale to you, but only in the context of that particular repository where you copied them to. If you also want them to be globally accessible, then CD into the repo that contains this file and run:

```bash
git repo-config-to-global
```

That will safely copy everything to  `.gitconfig` your home folder. (the one thats read by `git config --global ...`);

# Disclaimer
...only works on *nix style OS such as:

- MacOs
- Git bash
- Linux
- Unix
- ...

# Contribute
Use the GitHub issues to comment and share your own alias gems.
