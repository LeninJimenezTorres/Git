# GIT

## ACCESS TO GIT CONFIGURATION
```markdown
    git config
```

## CREATE A LOCAL REPOSITORY
```markdown
    git config --global user.name "My local repository"
    git config --global user.email "user@gmail.com"
```

## TO CHECK THE CURRENT CONFIGURATION FILE
```markdown
    git config --edit --global
```

## TO CHANGE THE CODE EDITOR
```markdown
    git config --global core.editor "code  --wait  --new-window"
                                     [__]  [____]  [___________]
                                       |      |          |__________ to open the file always in a new window
                                       |      |_____________________ to wait until the current opened window will be closed to use the git bash again
                                       |____________________________ the code editor name or location
```

## GIT VERSION
```markdown
    git --version
```

## GIT LOG
To view the commits history 
```markdown
    git log
    git log --oneline -> to show in one line abstract
    git log -1 HEAD
    
```

## GIT CHECKOUT
To revet to the previous version of all the repository
```markdown
    git checkout -- .
```
To create a new branch
```markdown
    git checkout -b NewBranchName
    git branch NewBranchName
```
To change to other branch
```markdown
    git checkout BranchName
```
To delete a branch branch
```markdown
    git checkout -d BranchName
```

## GIT BRANCH
To see all existent branch
```markdown
    git branch
```

## GIT RENAME MAIN BRANCH
To change the main branch name
```markdown
    git branch -M NewNameMainBranch
```

## GIT RENAME BRANCHES
To change the branch name
```markdown
    git branch -m OldBranchName NewBranchName
```


## GIT CREATE AN ALIAS
```markdown
    git config --global  alias.co  checkout
                              [_]  [______]
                               |       |_______ The command to create the alias
                               |_______________ The alias name
```


## GIT MERGE BRANCHES
To merge two branches, inside the one you want to pull the info:
```markdown
    git merge BranchName
```


## GIT AMEND
To change the last commit description 
```markdown
    git commit --amend 
```


## INITIALIZE A LOCAL REPOSITORY
To do this you need to be in the directory that you want to make the backup and after enter the following command
```markdown
    git init
```

## ACCESS TO ADD DOCUMENTS TO THE REPOSITORY
After you will enter in the directory and the before command, you will to add manually the files that you want to make the backup. To do this you can add one by one or all at the same time
```markdown
    command: git add file1.sh
    description: to add one by one file/directory
    
    command: git add .
    description: all in the current directory
```

## TO 
THE FILE TO THE COMMIT STORAGE / LOCAL REPO
```markdown
    command: git commit file1.sh
    description: After of enter this command your code editor will be opened and you can add a comment or message.
    
    command git commit -m "This is the message of the new commit"
    description: With this command your code editor will not open and the message will be added to the commit
    
    command gir commit -am "Commit description"
    description: This command simplify the [git add .] + [git commit -m 'commit description']
```

## TO SEE THE STATUS
```markdown
    git status
```

## TO IGNORE FILES OR DIRECTORIES
To ignores files or directories you need to create the file: `.gitignore` and inside of this file you have to add the files or directories you want to ignore
```markdown
    .gitignore
        file1.sh
        directoryA/
```

## TO IGNORE CHANGES OF A FILE/DIRECTORY
```markdown
    git checkout -- [filename]
```
the command include a space before and after of the `--`


## REMOTE ACCESS
```markdown
    command: git remote add origin  https://github.com/LeninJimenezTorres/Project/
    command: git push -u origin master
                                [____]
                                   |______ The branch inside which you want to make the backup
```

## FORCE A PUSH
```markdown
    git push --force upstream new-feature -> This will push the latest commits and overwrite any conflicting commits onto the upstream remote repository. 
```

## TO CHANGE THE REMOTE REPOSITORY
```markdown
    git remote set-url origin https://github.com/LeninJimenezTorres/Project/ 
```

## TO SEE THE REMOTE REPOSITORY
```markdown
    git remote -v 
```

## SSH ACCESS
Firt you need to verify local ssh keys. To do this you need enter the command:
```markdown
    ls -al ~/.ssh
```

## TO SEE DIFFERENCES
To see the differences between the current and the backup file you have to enter the command:
```markdown
    git diff file1.sh
             [______]
                 |______ file name and extention included
```

## MANAGE DIFFERENT VERSIONS
You can modify and create different versions of a same directory.
```markdown
    command: git branch
    description: to see all branches or versions
    
    command: git branch NewVersion
    description: with this you can create a new branch to new code versions
    
    command: git checkout NewVersion
    description: with this you can choose the version to work inside.
```


# TAGGING
To display all tags
```markdown
    git tag
```
To display a determinated tag
```markdown
    git tag -l 'tagname'
    git show tagname
```
To create a tag
```markdown
    git tag -a 'tagname' -m 'tag description'
```


# DEBUGGING
Depuration
Git has a couple of commands that are used to help debug a problem in your code. This ranges from figuring out where something was introduced to finding out who introduced it. 

To find changes in a file locating the specific line.  
```markdown
    git blame filename.txt
    git blame -L 1,10 README.md  -> It lets you inspect the first 10 lines of the README.md file to see when each line was last modified and who the author of the modifications was. 
```


### Support or Contact
Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
