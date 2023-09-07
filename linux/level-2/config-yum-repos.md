# Configure Local Yum repos

The `Nautilus` production support team and security team had a meeting last month in which they decided to use local yum repositories for maintaing packages needed for their servers. For now they have decided to configure a local yum repo on `Nautilus Backup Server`. This is one of the pending items from last month, so please configure a local yum repository on `Nautilus Backup Server` as per details given below.

a. We have some packages already present at location `/packages/downloaded_rpms/` on `Nautilus Backup Server`.

b. Create a yum repo named `yum_local` and make sure to set `Repository ID` to `yum_local`. Configure it to use package's location `/packages/downloaded_rpms/`.

c. Install package `wget` from this newly created repo.

**CheckCompleteIncomplete**
---

1. Create YUM Repo Config for local repo
   `sudo nano /etc/yum.repos.d/local_yum.repo`
   
2. Add config:
   ```yaml
    [local_yum]
    name=Local YUM Repository
    baseurl=file:///packages/downloaded_rpms/
    enabled=1
    gpgcheck=0
    ```
3. Update cache for config awareness
   `sudo yum makecache`
4. Install `wget`
   `sudo yum install wget`

--- 
CONGRATULATIONS!!!!
You have successfully completed the challenge.Results have been saved. Ref ID:64072016741b204d59fbe99c