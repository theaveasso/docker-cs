# docker-cs 
### What is Docker?

- **What is a container and what problems does it solve?**
- **Container repository - Where do containers live**
- **Before and After Container**
### What is Container?
- **What is a container?**
### Docker vs Virtual Machine
- **Difference between Docker and Virtual Machine**
### Docker Commandline Interface CLI
#### Container management Commands
- build an image
```bash
docker build [optins] .
  -t "app/container_name"
```
- create the container
```bash
docker create [options] IMAGE
  -a, --attach                # attach stdout, stderr
  -i, --interactive           # attach stdin (interactive)
  -t, --tty                   # pseudo-tty
    , --name                  # name your image
  -p, --publish 5000:5000     # port map
    , --expose 5432           # expose a port to linked containers
  -P, --publish-all           # publish all port
    , --link container:alias  # linking
  -v, --volume pwd:/app     # mount (absolute paths needs)
  -e, --env NAME=hello        # env vars
```
- run the container
```bash
docker run [options] IMAGE
  # see `docker create` for options
```
- start the container 
```bash
docker start [container ID or NAME]
```
- stop the container
```bash
docker stop [container ID or NAME]
```
- kill the container
```bash
docker kill [container ID or NAME]
```
- suspend the container
```bash
docker pause [container ID or NAME]
```
- resume the container
```bash
docker unpause [container ID or NAME]
```
- destroy the container
```bash
docker rm -f [container ID or NAME]
```
#### Inspecting the Container
- list running containers
```bash
docker ps
```
- list all containers
```bash
docker ps -a
```
- show the container output (stdout, stderr)


### Debugging Container
