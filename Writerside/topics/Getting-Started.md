# Getting Started

## Configuring git on our local machine
**Set your username and email address, which will be associated with your commits**:
```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```
## Setting up a new repository
* ``git init:`` Initialize a new repository
```Bash
git init
```
* ``git clone:`` Clone an existing repository
```Bash
git clone
```
* ``git status:`` Shows the current status of the working directory (modified, staged files, etc.)
```Bash
git status
```

## Saving changes a new file

1. Initialize a Git Repository (if not already done) 
    If your project isn't already a Git repository, navigate to your project directory and run:
```Bash
git init
```
2. Create or Add a New File, 
   Create a new file using your preferred text editor or the command line. For example, to create a new file named example.txt with some content:

```Bash
git add example.txt
```

3. Check the Status of Your Repository o see the current state of your repository and check for any untracked files, run:
```Bash
   git status
```
This command will display information about untracked files, changes not staged for commit, and changes to be committed.
   
4. Stage the New File, To add the new file to the staging area, use the git add command:

```Bash
git add example.txt
```
This command stages the file, preparing it to be committed.

5. Commit the Staged File, nce the file is staged, commit it to the repository with a descriptive message:

```Bash
git commit -m "Add example.txt file"
```
This command records the changes in the repository's history.

6. Push the Commit to a Remote Repository

If you're working with a remote repository (e.g., on GitHub), push your commit to the remote server:

```Bash
git push origin main
```
By following these steps, you can effectively save a new file in your Git repository.

## Tags and Versioning
* **git tag <tag_name>**: Adds a tag to mark a specific point in the history (e.g., for versioning). Example:
```Bash
git tag v1.0.0
```
* **git push origin --tags**: Pushes all tags to the remote repository. Example:
```Bash
git push origin --tags
```

## Undoing changes
``git clean``:

The ``git clean`` command is used to remove untracked files from your working directory. This is particularly useful when you have files that are not being tracked by Git and you want to clean up your working directory.

**Usage**:
* Dry Run (Preview Files to Be Removed):
```Bash
* git clean -n
```
* Remove Untracked Files:
```Bash
git clean -f
```
* Remove Untracked Files and Directories:
```Bash
git clean -fd
```
* Remove Ignored Files:
```Bash
git clean -fx
```

This command will remove all ignored files. Be cautious with this option as it will delete files listed in your .gitignore.

[//]: # (**Warning**: git clean permanently deletes files. Use it cautiously, especially if there are untracked files you may want to keep.)