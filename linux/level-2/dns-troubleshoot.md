# DNS Troubleshooting

The system admins team of xFusionCorp Industries has noticed intermittent issues with DNS resolution in several apps . `App Server 2` in `Stratos Datacenter` is having some DNS resolution issues, so we want to add some additional DNS nameservers on this server.

As a temporary fix we have decided to go with Google public DNS (ipv4). Please make appropriate changes on this server.

1. SSH into App Server 2
   `ssh steve@stapp02`
2. Edit `resolv.conf`
   `sudo vim /etc/resolv.conf`
   ```yaml
   nameserver 8.8.8.8
   nameserver 8.8.4.4
   ```

---

CONGRATULATIONS!!!!
You have successfully completed the challenge.Results have been saved. Ref ID:64072020741b204d59fbe9aa
