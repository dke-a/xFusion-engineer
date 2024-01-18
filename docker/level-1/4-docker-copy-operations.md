# Docker Copy Operations

The Nautilus DevOps team has some confidential data present on `App Server 1` in `Stratos Datacenter`. There is a container `ubuntu_latest` running on the same server. We received a request to copy some of the data from the docker host to the container. Below are more details about the task:

On `App Server 1` in `Stratos Datacenter` copy an encrypted file `/tmp/nautilus.txt.gpg` from docker host to `ubuntu_latest` container (running on same server) in `/opt/` location. Please do not try to modify this file in any way.

---

## SSH into App Server 1

```bash
ssh tony@172.16.238.10
```

## Copy file from host to container

```bash
sudo docker cp /tmp/nautilus.txt.gpg ubuntu_latest:/opt/
```

## Verify if file was copied

```bash
sudo docker exec -it ubuntu_latest ls /opt/
```

![](images/20240117231000.png)

---

You have successfully completed the challenge.Results have been saved. Ref ID:64072037741b204d59fbe9c9