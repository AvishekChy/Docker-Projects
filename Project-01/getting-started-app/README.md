# Project-01
This project is based on the familiarization on Docker and Dockerfile.

## Cloning the repository:

```bash
git clone https://github.com/docker/getting-started-app
```
-----

Now creating a `Dockerfile` to create an image of the getting started image container. In this `Dockerfile` the following codes are written to run the Image:

- Using node base image of version 18-alpine:
  
```dockerfile
FROM node:18-alpine
```
- Using the `/app` as working directory:
  
```dockerfile
WORKDIR /app
```
> The WORKDIR instruction sets the working directory for any RUN, CMD, ENTRYPOINT, COPY and ADD instructions that follow it in the Dockerfile.

- Using `COPY` to copy the files into the Image:
  
```dockerfile
COPY . . 
```
>  The first dot means source directory and The second dot means the destination directory
