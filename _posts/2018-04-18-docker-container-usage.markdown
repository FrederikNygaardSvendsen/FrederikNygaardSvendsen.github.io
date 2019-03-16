---
layout: post
title:  "docker container usage"
date:   2018-04-18 23:49:34 +0100
categories: docker
---
# Executing bash on a running docker container
To access the /bin/bash of a running docker container, run the following command:

    sudo docker exec -i -t <ContainerID> /bin/bash
    
# Analysing memory
When analyzing memory usage inside the linux container, the following file may be interesting:

    cat /sys/fs/cgroup/memory/memory.stat

# Other
To see usage (cpu/ram) of the docker contianer, docker stats can be helpful.