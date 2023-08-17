# Clone Repositories

DevOps team created a new Git repository last week; however, as of now no team is using it. The Nautilus application development team recently asked for a copy of that repo on `Storage server` in Stratos DC. Please clone the repo as per details shared below:

1. The repo that needs to be cloned is `/opt/demo.git`

2. Clone this git repository under `/usr/src/kodekloudrepos` directory. Please do not try to make any changes in the repo.

---

1. SSH into Storage Server
   `ssh natasha@ststor01.stratos.xfusioncorp.com`

2. CD into `cd /usr/src/kodekloudrepos`

3. Clone repo
   `git clone /opt/demo.git`