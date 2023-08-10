# Linux User Files

There was some users data copied on `Nautilus App Server 3` at `/home/usersdata` location by the `Nautilus` production support team in `Stratos DC`. Later they found that they mistakenly mixed up different user data there. Now they want to filter out some user data and copy it to another location. Find the details below:

On `App Server 3` find all files (not directories) owned by user `james` inside `/home/usersdata` directory and copy them all `while keeping the folder structure` (preserve the directories path) to `/media` directory.

1. Check /media

2. Find files as required and copy files along with directory structure
   `find /home/usersdata -user james -type f -exec cp --parents \{\} /media \;`
   
   ![](images/20230809222115.png)

---

You have successfully completed the challenge.Results have been saved. Ref ID:64072000741b204d59fbe97e