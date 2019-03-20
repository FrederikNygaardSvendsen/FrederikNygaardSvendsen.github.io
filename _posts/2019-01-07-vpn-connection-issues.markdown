---
layout: post
title:  "Issues connecting to VPN"
date:   2019-01-07 23:49:34 +0100
categories: vpn
---
I had issues connecting to VPN, and found out that an old "Secret" file, with an old password, was still lying around and was the one being used. Found solution on forum:


*You seem to have a collection of secrets files from multiple connections that haven't been cleaned up when the corresponding connection is stopped. Issue the following to clean things up :*

```
  sudo rm -f /etc/ipsec.d/nm-l2tp-ipsec-*.secrets
```

To debug the connection to vpn, use:
```
journalctl --follow
```