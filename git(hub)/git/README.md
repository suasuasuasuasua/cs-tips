# git

> **DO THE FIRST TWO ON A NEW MACHINE**

## Git Config

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
git commit [-m] "Commit message" # -m to add a commit message
```

## Creating Repos on GitHub

1. Go to [GitHub](github.com).
2. Click _new_ repo on the top left.
3. Give the repository a name.
4. Make it public or private (be smart)
5. Click create repository

## Cloning Repos

```bash
# Get the SSH link from Github (NOT THE HTTP ONE)
git clone git@github.com:<username>/<repo-name>.git
```

## Pushing and Pulling Changes

```bash
# Connect local repo to the remote repository on GitHub
# Grab this link from GitHub Repo > SSH > link
git remote add origin git@github.com:<username>/<repo-name>.git
# Set upstream branch so that we can push LOCAL changes to REMOTE repository
# Might be main or master
git push --set-upstream origin main
# OR
git push origin main
```

## .gitignore

1. Create a file called `.gitignore` at the root of the repository
2. Look at the [.gitignore templates](https://github.com/github/gitignore)
3. Copy and paste the one you need based on the repository languages
