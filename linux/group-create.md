# Create Group

There are specific access levels for users defined by the `xFusionCorp Industries` system admin team. Rather than providing access levels to every individual user, the team has decided to create groups with required access levels and add users to that groups as needed. See the following requirements:

a. Create a group named `nautilus_developers` in all App servers in `Stratos Datacenter`.

b. Add the user `mohammed` to `nautilus_developers` group in all App servers. (create the user if doesn't exist).

SSH into each app server and enter following commands:

1. `sudo groupadd nautilus_developers`
2. `sudo useradd mohammed`
3. `sudo usermod -aG nautilus_developers mohammed`

stapp01	172.16.238.10	stapp01.stratos.xfusioncorp.com	tony	Ir0nM@n	Nautilus App 1
stapp02	172.16.238.11	stapp02.stratos.xfusioncorp.com	steve	Am3ric@	Nautilus App 2
stapp03	172.16.238.12	stapp03.stratos.xfusioncorp.com	banner	BigGr33n	Nautilus App 3

---

Very manual process. A script could be created to automate this process especially if there are a huge number of servers.
