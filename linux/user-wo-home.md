# Linux User Without Home

The system admins team of `xFusionCorp Industries` has set up a new tool on all app servers, as they have a requirement to create a service user account that will be used by that tool.

Create a user named `kirsty` in `App Server 1` without a home directory.

1. SSH into Server App 1
   `ssh -i tony@172.16.238.10`
2. Add with -M option
   `sudo useradd -M kirsty`

---
You have successfully completed the challenge.Results have been saved. Ref ID:64071ffe741b204d59fbe97b

