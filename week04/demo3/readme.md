## Demo3 Python
In this demo we are going to build a new image from a Dockerfile using base image

### 1.create a directory
```bash
$mkdir demo3
$cd demo3
``` 
### 2.create a Dockerfile
create a Dockerfile for the following code
```Dockerfile
# Dockerfile
FROM python:3.7-alpine
CMD ["python","--version"]
```
* ```FROM python:3.7-alpine``` from python image tag ```3.7-alpine```
* ```CMD ["python","app.py"]``` start a new process using bash command ```$python --version```


### 3.build an image
create a new image locally and name it as ```2023_dsi321``` and tag ```1.0``` using the Dockerfile in current directory(.)
```bash
$docker build -t 2023_dsi321:1.0 .
```

### 4.spawn container from image
start a container from the image. ```-it``` is interactive mode. ```--rm``` is remove container when process stop.
```bash
$docker run -it --rm 2023_dsi321:1.0
```
