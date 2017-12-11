---
layout: post
title: Set Fedora based system to boot to run level 3 
---

To set Fedora based systems to boot into run level 3 (non graphical mode) run

```sh
sudo systemctl set-default multi-user.target
reboot
```

