# `git` tips

## Git Config

> **DO THE FIRST TWO ON A NEW MACHINE**

```bash
git config --global user.name "Your Name"
git config --global user.email "yourname@example.com"
git config --global init.defaultBranch main
git config --global color.ui auto
git config --global submodule.recurse true
```

## Set up SSH for Git

```bash
# Generate SSH key on local computer
# Remember to replace <youremail> (no carets)
ssh-keygen -t ed25519 -C <youremail>
# GitHub -> Settings -> SSH and GPG keys -> New SSH Key
# Copy and paste this
cat ~/.ssh/id_ed25519.pub
```

## Creating Git Repos LOCALLY

```bash
# create local git repo in current folder
git init
# tell git to track all files and folders in folder
git add .
# commit all changes
git commit
```

## Creating Repos on GitHub

1. Go to [GitHub](github.com).
2. Click _new_ repo on the top left.
3. Give the repository a name.
4. Make it public or private (be smart)
5. Click create repository

## Cloning Repos

```bash
# Get the SSH link from Github
git clone git@github.com:<username>/<repo-name>.git
```

## Pushing and Pulling Changes

```bash
# Connect local repo to the remote repository on GitHub
git remote add origin git@github.com:<username>/<repo-name>.git
# Set upstream branch so that we can push LOCAL changes to REMOTE repository
# It might be 'master' or 'main', but if we run very first code block on the README, it will be 'main'
git push --set-upstream origin main
# OR
git push origin main
```
