### configuration
    git config --global user.email ""
    git config --global user.name ""

### Create a new repository on the command line
    git init
    git add -A
    git status
    git commit -m "first commit"
    git branch -M main
    git remote add origin _url
    git push -u origin main

### Push an existing repository from the command line

    git remote add origin _url
    git branch -M main
    git push -u origin main


### git clone project
    git clone _url

### fatal: remote origin already exists.
    git remote remove origin



### Remove the history from 
    rm -rf .git

### Change Git repository
    git remote set-url origin _url

    
### ! [rejected] master -> master (fetch first)
error: failed to push some refs to 'git@github.com:zapnaa/abcappp.git'
    git fetch origin main
    git merge origin main
    git push origin main --force

### Update date
    GIT_COMMITTER_DATE="Wed Feb 16 14:00 2011 +0100" git commit --amend

### Bring back any committed code
    git cherry-pick -e <Commit_ID>
