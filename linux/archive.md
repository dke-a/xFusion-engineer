# Archive

On `Nautilus` storage server in `Stratos DC`, there is a storage location named `/data`, which is used by different developers to keep their data (non confidential data). One of the developers named `james` has raised a ticket and asked for a copy of their data present in `/data/james` directory on storage server. `/home` is a FTP location on storage server itself where developers can download their data. Below are the instructions shared by the system admin team to accomplish this task.

a. Make a `james.tar.gz` compressed archive of `/data/james` directory and move the archive to `/home` directory on Storage Server.

1. `ssh natasha@172.16.238.15`
2. `sudo tar -czvf /home/james.tar.gz james`
   
---

You have successfully completed the challenge.Results have been saved. Ref ID:64072027741b204d59fbe9b3

