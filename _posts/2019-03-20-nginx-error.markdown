---
layout: post
title:  "NGINX Error"
date:   2019-03-20 23:49:34 +0100
categories: nginx network
---
I had an issue with NGINX returning 502 Bad Gateway. See the log files by going to:


```
  /var/log/nginx/error.log
```

The NGINX configuration itself can be found here:

```
  /etc/nginx/nginx.conf
```

In my case, restarting the NGINX service fixed the problem