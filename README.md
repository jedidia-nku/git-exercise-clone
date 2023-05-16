## Bundle 4

### Exercise 1

```bush
Switched to branch 'main'
M       README.md
  (use "git push" to publish your local commits)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git remote add git-copy  https://github.com/jedidia-nku/git-exercise-clone.git     
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git remote
git-copy
origin
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add --all
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit -m "add new changes to home page"
[main d106378] add new changes to home page
 2 files changed, 50 insertions(+), 1 deletion(-)
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 965 bytes | 80.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
   43213ec..d106378  main -> main
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push git-copy
Enumerating objects: 23, done.
Counting objects: 100% (23/23), done.
Delta compression using up to 2 threads
Compressing objects: 100% (22/22), done.
Writing objects: 100% (23/23), 5.96 KiB | 381.00 KiB/s, done.
Total 23 (delta 8), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (8/8), done.
To https://github.com/jedidia-nku/git-exercise-clone.git
 * [new branch]      main -> main
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> 
```

### exercise 2

```bush
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout -b ft/footer
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add footer.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit -m "add a footer page"
[ft/footer a9d89a3] add a footer page
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 footer.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add --all
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit -m "feat: add new changes to the footer page"
[ft/footer b73d893] feat: add new changes to the footer page
 2 files changed, 39 insertions(+), 549 deletions(-)
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> ^C
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push --set-upstream origin ft/footer
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
merge: squash - not something we can merge
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git merge --squash ft/footer 
Updating d106378..b73d893
Squash commit -- not updating HEAD
 README.md   | 577 +++---------------------------------------------------------
 footer.html |  11 ++
 2 files changed, 39 insertions(+), 549 deletions(-)
 create mode 100644 footer.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit -m "footer changes squashing"
[ft/squashing 1d84378] footer changes squashing
 2 files changed, 39 insertions(+), 549 deletions(-)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push 
fatal: The current branch ft/squashing has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/squashing

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push --set-upstream origin ft/squashing
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 916 bytes | 101.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/jedidia-nku/Gym-Git-Exercise-Solution/pull/new/ft/squashing
remote:
To https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise>   
```
