git clone https://github.com/mentacity/class.git
cd class
git branch (only shows master)
git branch -r (shows all remote branches)
git checkout SB1.1
git branch new-SB1.1 (creates a branch of SB1.1)
git checkout new-SB1.1 (switch to the new branch)
git branch -r (shows the new branch is not on the remote)
git push -u (First attempt I had to use: git push -u origin my_branch)


## Time to test
- edit a local file
- commit
- push

git branch
git status
git add (* for all or the specific filename)
git status
git commit -m "whatever commit message you choose"
git push -u

### What this should do, is add the code to my new branch 
With github I can look and see if the change is on the remote

