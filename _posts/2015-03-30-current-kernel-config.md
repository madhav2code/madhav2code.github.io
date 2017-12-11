---
layout: post
title: How to get current Kernel config
---

Here is how you get the current running configuration

* cat /proc/config.gz > config.gz
* gunzip config.gz 
* “config” will have your current configuration
