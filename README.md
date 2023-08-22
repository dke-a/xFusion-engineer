README
======

**KodeKloud Engineer** is a development program where real tasks are performed on real systems as part of a fictional company called xFusion Corp.

Tasks that are performed provide skills experience for roles such as Systems Administrator, DevOps Engineer and Architect.

| Systems Administrator       	| Devops Engineer                                    	| Devops Architect                                   	|
|-----------------------------	|----------------------------------------------------	|----------------------------------------------------	|
| Linux System Administration 	| Deploy multi-tier applications Troubleshoot Issues 	| Design & Build Cl/CD Pipelines                     	|
| Users & Groups              	| Develop Automation Playbooks                       	| Design & Build Kubernetes Clusters                 	|
| Filesystems                 	| Build CI/CD Pipelines                              	| Design & Develop Automation Solutions              	|
| Storage, LVM                	| Containerize Applications                          	| Guiding Systems Administrator and DevOps Engineers 	|
| Packages                    	| Build Container Clusters                           	| Troubleshooting Complex Topics                     	|
| Services                    	| Deploy Monitoring Solutions                        	|                                                    	|
| Networking                  	| Regular Maintenance Activities                     	|                                                    	|
| IPTables                    	| Guiding Systems Administrators                     	|                                                    	|
| Firewalls                   	|                                                    	|                                                    	|
| Deploy Simple Applications  	|                                                    	|                                                    	|

<!-- ![Roles and Responsibilities](images/20230718230127.png) -->

---
## LINUX LEVEL 1

| **Task Number** | **Title**                                                                           | **Accomplishment**                                                        | **Tags**                                   |
|-----------------|-------------------------------------------------------------------------------------|---------------------------------------------------------------------------|--------------------------------------------|
| 1               | [Linux File Permissions](linux/file-permissions.md)                                 | SSH into App Server to change file permissions to be executable.          | `File Operations` `Linux` `SSH`            |
| 2               | [Create a User](linux/user-create.md)                                               | Create user in App Server and adjust user group.                          | `Linux` `SSH` `Users & Groups`             |
| 3               | [Create a Group](linux/group-create.md)                                             | Create group in all App servers. Add user to group.                       | `Linux` `SSH` `Users & Groups`             |
| 4               | [Create a Linux User with Non-interactive Shell](linux/non-interactice-terminal.md) | Create user in App Server 1.                                              | `Linux` `SSH` `Users & Groups`             |
| 5               | [Linux User Without Home](linux/user-wo-home.md)                                    | Create user without a home directory.                                     | `Linux` `SSH` `Users & Groups`             |
| 6               | [Linux User Expiry](linux/user-expiry.md)                                           | Create user with expiry                                                   | `Linux` `SSH` `Users & Groups`             |
| 7               | [Linux User Files](linux/user-files.md)                                             | Copy user files into another directory while keeping directory structure. | `Linux` `SSH` `Users & Groups`             |
| 8               | [Disable Root Login](linux/disable-root-login.md)                                   | Disable root login on all app servers                                     | `Linux` `SSH`                              |
| 9               | [Linux Archives](linux/archive.md)                                                  | Archive user data in storage folder                                       | `File Operations` `Linux` `SSH`            |
| 10              | [Access Control Lists](linux/access-control-list.md)                                | Modify file permissions and ACL.                                          | `File Operations` `Linux` `Users & Groups` |
| 11              | [String Substitute](linux/string-substitute)                                        | Substitute strings in an XML file.                                        | `File Operations` `Linux`                  |
| 12              | [Cron Schedule to Deny Users](linux/cron-schedule-deny.md)                          | Update CRON settings to deny and allow users.                             | `CRON` `Linux`                             |
| 13              | [Run Levels](linux/run-levels.md)                                                   | Change default run level of all app servers to GUI.                       | `Linux` `Run Levels`                       |
| 14              | [NTP Setup](linux/NTP.md)                                                           | Setup NTP and modify config to sync time with other servers.              | `Linux` `NTP`                              |
| 15              | [Firewalld Rules](linux/firewalld-rules.md)                                         | Open connection on public zone TCP port 8083.                             | `Firewalld` `Linux`                        |
| 16              | [Resource Limits](linux/resource-limits.md)                                         | Add soft and hard limit for running user processes on server.             | `Linux` `User Processes`                   |



## GIT LEVEL 1

| **Task #** | **Title**                                                  | **Accomplishment**                                                                                 | **Tags**           |
|------------|------------------------------------------------------------|----------------------------------------------------------------------------------------------------|--------------------|
| 1          | [Install and Create Bare Repository](git/level-1/setup.md) | Create bar Git repo in Storage Server                                                              | `Git` `Initialize` |
| 2          | [Clone Repositories](git/level-1/clone-repo.md)            | Clone Git repo in Storage Server                                                                   | `Clone` `Git`      |
| 3          | [Fork a Repo](git/level-1/fork-repo.md)                    | Fork Repo in Gitea                                                                                 | `Fork` `Git`       |
| 4          | [Repo Update](git/level-1/repo-update.md)                  | Copy file from jump server to storage server. Add, commit, and push updated repo in storage server | `Git`              |
| 5          | [Delete Branch](git/level-1/delete-branch.md)              | Delete branch in storage server                                                                    | `Branch` `Git`     |
