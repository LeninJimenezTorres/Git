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

## INITIALIZE A LOCAL REPOSITORY
To do this you need to be in the directory that you want to make the backup and after enter the following command
```markdown
    git init
```

## ACCESS TO ADD DOCUMENTS TO THE REPOSITORY
After you will enter in the directory and the before command, you will to add manually the files that you want to make the backup. To do this you can add one by one or all at the same time
```markdown
    one by one: `git add file1.sh`
    all in the current directory: `git add .`
```

### Support or Contact
Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
