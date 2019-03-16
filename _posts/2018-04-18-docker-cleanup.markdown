---
layout: post
title:  "docker cleanup"
date:   2018-04-18 23:49:34 +0100
categories: docker
---
# Cleaning up in docker
when wanting to cleanup untagged docker images, this command can be run

	docker rmi $(docker images | grep "^<none>" | awk "{print $3}")