# Collaborative Directories

The Nautilus team doesn't want its data to be accessed by any of the other groups/teams due to security reasons and want their data to be strictly accessed by the `dbadmin` group of the team.

Setup a collaborative directory `/dbadmin/data` on `app server 3` in `Stratos Datacenter`.

The directory should be group owned by the group `dbadmin` and the group should own the files inside the directory. The directory should be `read/write/execute` to the user and group owners, and `others` should not have any access.

---

1. SSH into App Server 3
   `ssh banner@stapp03`
2. Create directory
   `sudo mkdir -p /dbadmin/data`
3. Change ownership
   `sudo chown :dbadmin /dbadmin/data`
4. Modify permissions
   `sudo chmod 770 /dbadmin/data`
5. Modify permissions for new files to inherit group ownership
   `sudo chmod g+s /dbadmin/data`
