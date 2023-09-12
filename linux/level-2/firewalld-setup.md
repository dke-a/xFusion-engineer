# Firewalld Setup

To secure our `Nautilus` infrastructure in `Stratos Datacenter` we have decided to install and configure `firewalld` on all app servers. We have Apache and Nginx services running on these apps. Nginx is running as a reverse proxy server for Apache. We might have more robust firewall settings in the future, but for now we have decided to go with the given requirements listed below:

a. Allow all incoming connections on Nginx port, i.e `80`.

b. Block all incoming connections on Apache port, i.e `8080`.

c. All rules must be permanent.

d. Zone should be public.

e. If Apache or Nginx services aren't running already, please make sure to start them.

---

1. Check status of `apache`/`httpd` and `ngnix` service
   `sudo systemctl status httpd`

2. Install `firewalld`
   `sudo yum install firewalld -y`

3. Start `firealld`
   `sudo systemctl start firewalld`

4. Add rules
   ```bash
    sudo firewall-cmd --permanent --zone=public --add-port=80/tcp
    sudo firewall-cmd --permanent --zone=public --add-port=8080/tcp --reject
   ```
5. Allow incoming connections to ngnix port
   `sudo firewall-cmd --permanent --zone=public --add-service=http`

6. Block connections on apache port
   `sudo firewall-cmd --permanent --zone=public --remove-port=8080/tcp`

7. Reload firewalld
   `sudo firewall-cmd --reload`

8. Ensure rules are set
   `sudo firewall-cmd --list-all`

---

CONGRATULATIONS!!!!
You have successfully completed the challenge.Results have been saved. Ref ID:6407201d741b204d59fbe9a6