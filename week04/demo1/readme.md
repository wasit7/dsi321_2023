## Demo1 Install Docker and test run
### 1.Setup Docker
* For Windows please install WSL and Docker for Desktop. Check the document here https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-containers
* For Ubunto use
```bash
$sudo apt-get update
$sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
```
### 2. Check Docker version
It is good the remember the Docker version current in use
```bash
$docker --version
```
### 3.Pull Image
Pull image(registry) from DockerHub to local manchine.
```bash
$docker pull hello-world
```
### 4.List Image
Show list of images in local machine
```bash
$docker images
```
### 5.Run Image
Use the image for spawning a container and run.
```bash
$docker run hello-world
```