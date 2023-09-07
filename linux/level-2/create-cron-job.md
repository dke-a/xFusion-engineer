# Create CRON Job

The `Nautilus` system admins team has prepared scripts to automate several day-to-day tasks. They want them to be deployed on all app servers in `Stratos DC` on a set schedule. Before that they need to test similar functionality with a sample cron job. Therefore, perform the steps below:

a. Install `cronie` package on all `Nautilus` app servers and start `crond` service.

b. Add a cron `*/5 * * * * echo hello > /tmp/cron_text` for `root` user.

---

1. SSH into app server
   `ssh tony@stapp01`
2. Install cronie
   `sudo yum install cronie -y`
3. Enable and start cronie. Check if it is running.
   ```bash
   sudo systemctl start crond
   sudo systemctl enable crond
   sudo systemctl is-active crond
   ```
4. Edit crontab for root
   `sudo crontab -u root -e`
5. Add the cron command:
   `*/5 * * * * echo hello > /tmp/cron_text`
6. (optional) Restart cron service
   `sudo systemctl restart crond`

Do for each other app server.

---
You have successfully completed the challenge.Results have been saved. Ref ID:64072021741b204d59fbe9ac