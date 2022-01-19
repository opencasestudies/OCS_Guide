# Contributor's Guide

## Version Control

### Making a New Branch

1. Go to the main branch and pull

```
git checkout main
git pull
```

2. Create new branch from main. Replace 'new_branch' with your desired branch name.

```
git checkout -b new_branch
```

Note: See list of current branches with ```git branch```

3. Add your changes to the content.

4. Commit changes to GitHub. 

```
git add name_of.file
git commit -m "commit message here"
git push
```

**Tip:** If you added a file that you do not want to commit to GitHub, use ```git reset name_of.file```. This works before or after commit, but must be before push. If the file has already been pushed, use ```git revert```.

**Tip:** If you want pull changes from main into your local branch, you may stash your changes first with ```git stash```. Then move to the main branch with ```git checkout main``` and ```git pull``` to make sure your local main branch is up to date. Go back to the branch you are working on with ```git checkout your_branch``` and use ```git merge main```. Use ```git stash pop``` to bring back your local changes from the stash. This may require you to resolve conflicts if there are any. 

### Resolving Conflicts

1. Move to the main branch and pull to make sure your local main branch is up to date.

```
git checkout main
git pull
``` 

2. Go back to the branch you are working on and merge with the main branch. 

```
git checkout your_branch
git merge main
```

3. Look in the files that git lists conflicts for. The conflicting lines will be highlighed as such:

```
<<<<<<< HEAD:file.txt
My local changes
=======
...
=======
Remote main branch version
>>>>>>>
```

Keep the parts you want to save and delete the parts that need to be removed. Once you are finished resolving conflicts, make sure to remove all the lines with "<<<<<<<", "=======", ">>>>>>>".

4. Add, commit and push changes.

```
git add your_file.name
git commit -m "commit message here"
git push
```

*Note:* If you need to remove a file both locally and remotely, use ```git rm your_file.name```. If the file needs to stay on your local system but be removed from the remote, use ```git rm --cached your_file.name```.



