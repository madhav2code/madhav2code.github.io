---
layout: post
title: Install Telnet server on Fedora 20
---

#### Steps to install Telnet server on Fedora 20

1. sudo yum install telnet-server xinetd –y
2. sudo systemctl enable telnet.socket
3. sudo systemctl start telnet.socket
4. sudo firewall-cmd --permanent --add-service=telnet
5. sudo firewall-cmd --reload
