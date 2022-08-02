# `bash` basics

## Generally Useful

- Tab for autocompletion
- `<Ctrl-l>` to clear the screen
- `code [-r] <file or folder>` to open file or folder in VSCode in new window; `-r` to open in same window

## Navigation

```bash
# Move to home directory at /~/
cd
# Move into a directory called 'folder1'
cd folder1
# Move one directory UP
cd ..
```

# Removing

```bash
# Remove a file
rm file1
# Can't remove a file normally
# Need to use recursive flag
# sudo if there are write/delete protected files
# BE CAREFUL BECAUSE YOU CANNOT GET THESE FILES BACK
[sudo] rm -r folder1
```

## Moving and Renaming

```bash
# To move around
mv my_file ./folder1/
# To rename
mv old_file_name new_file_name
```

## Installing packages

```bash
# Will need higher privileges for installing a package with apt
sudo apt install <package name>
```
