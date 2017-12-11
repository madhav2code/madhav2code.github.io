---
layout: post
title: Systemd mount unit 
---

Sample systemd mount unit

```sh
[Unit]
Description=Boot Directory

[Mount]
What=/dev/sda1
Where=/boot
Type=ext4
Options=ro,noatime,discard,data=ordered

```

