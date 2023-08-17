# NTP

The system admin team of `xFusionCorp Industries` has noticed an issue with some servers in `Stratos Datacenter` where some of the servers are not in sync w.r.t time. Because of this, several application functionalities have been impacted. To fix this issue the team has started using common/standard NTP servers. They are finished with most of the servers except `App Server 2`. Therefore, perform the following tasks on this server:

1. Install and configure NTP server on `App Server 2`.

2. Add NTP `server 3.pool.ntp.org` in NTP configuration on `App Server 2`.

3. Please do not try to start/restart/stop `ntp` service, as we already have a restart for this service scheduled for tonight and we don't want these changes to be applied right now.

---

1. `sudo yum install ntp`

2. `sudo nano /etc/ntp.conf`

3. add `server 3.pool.ntp.org` to the ntp.conf file

---

You have successfully completed the challenge.Results have been saved. Ref ID:6407200f741b204d59fbe992

