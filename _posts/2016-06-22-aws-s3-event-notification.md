---
layout: post
title: S3 bucket notification event
tags:
- AWS
- S3
- SNS
- SQS
- Lambda
---
S3 buckets can be configured to react to certain events, eg. objectcreated. S3 is then able to send an SNS or SQS event or even trigger a lambda. Pre- and postfix for filenames lets you narrow down which files to trigger events for.
