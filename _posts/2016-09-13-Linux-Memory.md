---
layout: post
title: Analyze memory usage, docker
tags:
- Linux
- Docker
- Memory
---
To access the /bin/bash of a running docker container, run the following command:


<!-- language: lang-none -->
    sudo docker exec -i -t <ContainerID> /bin/bash

When analyzing memory usage inside the linux container, the following file may be interesting:


<!-- language: lang-none -->
    cat /sys/fs/cgroup/memory/memory.stat

To see usage (cpu/ram) of the docker contianer, **docker stats** can be helpful.
