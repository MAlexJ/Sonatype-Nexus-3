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
ports:
    - 127.0.0.1:8888:8081

Run composition

```sh
docker-composer up -d
```
