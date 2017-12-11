---
layout: post
title: Logrotate HTTPD logs without restarting HTTPD service
---

Update /etc/logrotate.d/httpd to

```sh
/var/log/httpd/*log {
    copytruncate
    rotate 5
    size 1M
    missingok
    notifempty
    delaycompress
}
```

This will copy and truncate the original file