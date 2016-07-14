---
layout: post
title: Remove all untagged docker images
tags:
- Docker
---
when wanting to cleanup untagged docker images, this command can be run

<!-- language: lang-none -->
		docker rmi $(docker images | grep "^<none>" | awk "{print $3}")
