# Run Docker Container

Nautilus DevOps team is testing some applications deployment on some of the application servers. They need to deploy a nginx container on `Application Server 1`. Please complete the task as per details given below:

1. On `Application Server 1` create a container named `nginx_1` using image `nginx` with `alpine` tag and make sure container is in `running` state.

---

## SSH into App Server 1

```bash
ssh tony@172.16.238.10
```

### Create the nginx image

```bash
sudo docker run --name nginx_1 -d nginx:alpine
```