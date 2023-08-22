# Delete Branch

Nautilus developers are actively working on one of the project repositories, `/usr/src/kodekloudrepos/cluster`. They were doing some testing and created few test branches, now they want to clean those test branches. Below are the requirements that have been shared with the DevOps team:

On `Storage server` in Stratos DC delete a branch named `xfusioncorp_cluster` from `/usr/src/kodekloudrepos/cluster` git repo.

1. SSH into Storage Server
   `ssh natasha@ststor01`
2. Change into directory
   `cd /usr/src/kodekloudrepos/cluster`
3. Check git status
   `git status`
   ![](images/20230818215558.png)
4. Switch to master branch to delete `xfusioncorp_cluster`
   `sudo git checkout master`
5. Delete branch
   `sudo git branch -d xfusioncorp_cluster`

---


You have successfully completed the challenge.Results have been saved. Ref ID:6484acceea2ac6a485a3b140

