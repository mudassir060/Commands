# configration
git config --global user.email ""
git config --global user.name ""

# create a new repository on the command line
git init
git add -A
git status
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/mudassir060/OLX-PK.git
git push -u origin main
                
# push an existing repository from the command line

git remote add origin https://github.com/mudassir060/OLX-PK.git
git branch -M main
git push -u origin main


# get git project
git clone https://github.com/mudassir060/OLX-PK

# fatal: remote origin already exists.
git remote remove origin



# Remove the history from 
rm -rf .git



# ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'git@github.com:zapnaa/abcappp.git'
git fetch origin main
git merge origin main
git push origin main --force

# Update date
GIT_COMMITTER_DATE="Wed Feb 16 14:00 2011 +0100" git commit --amend

