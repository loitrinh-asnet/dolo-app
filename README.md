# Learning Docker 2nd
```Faster app development and deployment with Docker Containers```

[![N|Solid](https://dt-cdn.net/assets/images/content/resources/docker-c-0e3b80d791.png)](https://www.docker.com)

Getting started with Docker.
  - The key drivers for Dockerization
  - Differentiating between containerizatin and virtualization
  - Installing the Docker Engine
  - Some important concepts about docker hub, docker images, docker container and so on.

You can also:
  - Building docker images
  - Publishing docker images
  - And So on


### Installation
Just focus to install Docker on the MAC
Note that It is always recommended that you use Docker For Mac for supported OS X versions 10.10.3, Yosemite or newer.

```sh
1. Download Docker for Mac from the link
https://download.docker.com/mac/beta/Docker.dmg.
2. Double-click to download Docker.dmg and move it
[Show in here]
3. Double-click on Docker.app in Applications
It will install Docker Components
4. Finally, verify the Docker version
docker --version
```
### Docker
Building the image locally using the following command
```sh
cd dolo-app
docker build -t loitrinh/django-app:0.1.0 -f ./compose/django/Dockerfile .
docker build -t loitrinh/postgres:0.1.0 -f ./compose/postgres/Dockerfile .
```
Pushing all created images to Docker Hub using the following command
```sh
docker push loitrinh/django-app:0.1.0
docker push loitrinh/postgres:0.1.0
```
### Usage
```sh
cd dolo-app
docker-compose build
```
This will pull in the necessary images from docker hub named is loitrinh.

Once done, Run the docker-compose up command from the top level directory for your project.:

```sh
docker-compose up
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
localhost:8000
```
License
----
MIT
