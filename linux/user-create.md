# Create User

For security reasons the `xFusionCorp Industries` security team has decided to use custom Apache users for each web application hosted, rather than its default user. This will be the Apache user, so it shouldn't use the default home directory. Create the user as per requirements given below:


1. Check server details from [documentation](https://kodekloudhub.github.io/kodekloud-engineer/docs/projects/nautilus)

2. SSH into App Server 3
   `ssh banner@stapp03.stratos.xfusioncorp.com`

3. Add user
   `sudo adduser kirsty`

4. Edit UID and Directory
   `sudo usermod -u 1582 kirsty`
   `sudo usermod -d /var/www/kirsty kirsty`

---

You have successfully completed the quiz. Results have been saved. Ref ID:64688038c1ff5e7e05478dd8



BigGr33n