---
layout: post
title: Remember to check policies for lambda execution role
tags:
- AWS
- IAM
- Lambda
---
When the Lambda is being executed, it does so by assuming a role. If this role does not have permission to write to cloudwatch, no logs will be generated. No error of this will occur, logs simply wont appear. Allways remember to check for policies.
