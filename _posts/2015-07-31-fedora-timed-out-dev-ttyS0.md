---
layout: post
title: Timed out waiting for device dev-ttyS0.device
---

If you see this "Timed out waiting for device dev-ttyS0.device" during boot up make sure that ``` CONFIG_FHANDLE=y in /proc/config.gz ```

Else recompile your kernel with ``` CONFIG_FHANDLE=y ```
Newer versions of systemd requires a kernel with ``` CONFIG_FHANDLE=y set ```


