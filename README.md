# Sonatype-Nexus-3
Sonatype Nexus3 Docker

link to nexus: https://www.sonatype.com/products/repository-pro <br>
link to docker: https://hub.docker.com/r/sonatype/nexus3  <br>
how to use: https://www.youtube.com/watch?v=6WjwrZknYVk <br>

## How to use

```sh
git clone https://github.com/MAlexJ/Sonatype-Nexus-3.git
```

Change port in docker-compouse.yaml
```sh
ports:
    - 127.0.0.1:8888:8081
```    

Run composition

```sh
docker-composer up -d
```

## Information

Default user is **admin** and the uniquely generated password can be found in the **admin.password** file inside the volume. 
See Persistent Data for information about the volume.

1. go to the specified mount folder /NEXUS-DATA <br>
2. find the generated password in the admin.password file <br>
example:

```sh
..........\Sonatype-Nexus-3-main\nexus-data
λ cat admin.password
3e5a9a3d-7e5f-4412-9a4d-a5e42ef0eea8
```
3. change admin password for nexus
