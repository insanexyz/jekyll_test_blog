---
layout: post
title: Docker basic commands
date: 2025-07-27
categories: docker
author: insane
permalink: /posts/docker-basic-commands
---
Learn the most basic docker commands.

## What is docker?
Docker is used to make containers using a docker file.

## Install docker
Head to https://docs.docker.com/get-started/get-docker/ and simply follow the guide for your operating system.

If you are on Arch Linux then
```bash
sudo pacman -S docker   # Install docker - It includes docker cli frontend and a docker daemon backend to manage the docker containers.
systemctl start docker.service  # To start docker service immediately
systemctl enable docker.service # To start docker service automatically everytime you boot
```

##