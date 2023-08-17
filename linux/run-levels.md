# Linux Run Levels

New tools have been installed on the app servers in `Stratos Datacenter`. Some of these tools can only be managed from the graphical user interface. Therefore, there are some requirements for these app servers as below.

On all App servers in `Stratos Datacenter`, change the `default runlevel` so that they can boot in `GUI (graphical user interface)` by default. Please do not try to `reboot` these servers after completing this task.

1. SSH into each APP SERVER
2. `systemctl get-default`
   To get current target
3. `sudo systemctl set-default graphical.target`
   To set GUI target.

   ---

   You have successfully completed the challenge.Results have been saved. Ref ID:64072030741b204d59fbe9bf