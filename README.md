# GIT Cheat Sheet

## Set username and Email
```sh
git config --global user.name ""
git config --global user.email ""

git config --global -l  
```
## GIT baisc commands

### Create a git repository
Navigate to the folder where the repository wuill be created and execute the git command bellow
```sh
git init
```


### Check repository status
```sh
git status
```



### Exclude files you don't want to track
To exclude files from you commitments, add a .gitignore file and list the files and folders you wnat GIT to do not track
```sh
touch .gitignore
```

### To track an empty folde
To track an empty folder, add a blank .git-keep file in the folder
e.g. creating a folder assets and adding a .git-keep file in it
```sh
mkdir assets
cd assets
touch .git-keep
```

### Add all files to the list of files that you are tracking
```sh
git add .
```

### Add all untracked files to the list of files that you are tracking
```sh
git add -A
```

### Commit
```sh
git commit <file name | optional, if blamnk, will commit all files> -m 'This commig short description'
```

### Update the commit with the changes
```sh
git commit -a --amend --no-edit
```

### Check what was changed on files
```sh
git diff
```

### Get a list of commitments
```sh
git log --oneline
```

### Recover a deleted file
```sh
git checkout -- <the file to recover>
```

### Remove a file from tracking
```sh
git rm <the file to remove>
```

### to recover a file that was removed with ```git rm```
```sh
git reset HEAD <the file to recover>

git checkout -- <the file to recover>
```