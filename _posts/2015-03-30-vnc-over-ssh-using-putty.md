---
layout: post
title: VNC over ssh using putty
---

1. Download putty from [here](http://the.earth.li/~sgtatham/putty/latest/x86/putty.exe)
2. Run putty and connect to your VNC server
3. Click on “Change Settings” –>Connection–>SSH–>Tunnels
4. In “Add new forwarded port” –> Enter source port as 5901 and Destination as server-ip:5901
5. Click on Add button
6. Click on Apply button
7. Open VNC viewer and connect to localhost:1
