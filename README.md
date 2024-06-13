# AwesomeCTF

![asd](https://images.deepai.org/art-image/641133ca6e0b4225a309d03edadbd3dc/capture-the-flag-0a2df9.jpg)

## Welcome
Welcome to my awesomeCTF. AwesomeCTF is an easy, straight-forward CTF environment created in docker to allow easy and fast deployment.
The CTF contains a few flags which can be obtained by pwning each part of the challenge.
I Hope you enjoy!

## The environment
The challgenge was created in a docker environment as part of the question if it was possible to do so (and it is, kinda)
The environment contains two systems, a MySQL server and a Debian host:

AwesomeCTF   
    |-----awesomectf-host   
    |-----awesomectf-mysql   

The images are pre-created docker images which contain the neccesary files, applications and data.
This repository contains the docker-compose.yml files for both x86/x64 and ARM.

The docker-compose will pull the nsbyteone/awesomectf-host and nsbyteone/awesomectf-mysql images from the docker hub and start them properly.
No additional configuration is required.

## Getting started

Requirements:
- Docker Desktop
https://docs.docker.com/desktop/install/windows-install/
https://docs.docker.com/desktop/install/linux-install/   

Optional:   
- Git

Steps (with git installed):   
1. git clone https://github.com/NsByte/AwesomeCTF
2. cd AwesomeCTF
3. docker-compose -f docker-compose.yaml up --force-recreate
4. You should be able to reach two ports on your machine
5. Enjoy!

Steps (without git installed):
```
1. Download the file https://raw.githubusercontent.com/NsByte/AwesomeCTF/main/docker-compose.yaml
2. In that folder run 'docker-compose up --force-recreate'
3. Enjoy!
```

Stopping the environment:
docker-compose down -v
Starting the environment:
docker-compose -f docker-compose.yaml up --force-recreate

*TLDR:*    
git clone https://github.com/NsByte/AwesomeCTF && cd AwesomeCTF && docker-compose -f docker-compose.yaml up

## How do i win?
Get access to the docker host through vulnerabilities and elevate your privileges to root!
On this small journey you will collect some flags which can be evaluated at the end of the road.

## Help me daddy im stuck
Try harder

Enjoy!
