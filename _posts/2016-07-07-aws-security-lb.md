---
layout: post
title: AWS LoadBalancer security
tags:
- AWS
- LoadBalancer
- ACL
- SecurityGroup
---
When defining a LoadBalancer, it is associated to subnet. It is necessary for the ACL to allow inbound communication from this subnet, for requests to be able to hit the associated instance in the LoadBalancer The LoadBalancer should also have a SecurityGroup associated, same with the EC2 instance. The EC2's SecurityGroup should then allow incoming requests from the LoadBalancers SecurityGroup on the specified ports.
