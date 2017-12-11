---
layout: post
title: Mount Fedora cloud image to local directory
---

Steps to mount Fedora cloud image locally

* Dowload the latest image from https://getfedora.org/en/cloud/download/
* unxz Fedora-Cloud-Base-20141203-21.x86_64.raw.xz  --> This will replace the compressed image with an uncompressed one 
* Rename the file from Fedora-Cloud-Base-20141203-21.x86_64.raw to Fedora-Cloud-Base-20141203-21.x86_64.img
* Check if you have kpartx installed 
```sh
yum install kpartx -you
```

* kpartx -a Fedora-Cloud-Base-20141203-21.x86_64.img
* mkdir /mnt/fedora
* mount /dev/mapper/loop0p1  /mnt/fedora

Steps to un-mount

* umount /mnt/fedora
* kpartx -d Fedora-Cloud-Base-20141203-21.x86_64.img