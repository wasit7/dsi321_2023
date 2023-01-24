## Demo2 Run Ubuntu container
In this demo an Unbutu 14.04 is pulled to local machine and run bash
### Pull Image
Pull image from DockerHub
```bash
$docker pull ubuntu:trusty
```
### Run the container
```bash
$sudo docker run -it --rm ubuntu:trusty bash
```
### Check version of OS
```bash
$cat /etc/os-release
```