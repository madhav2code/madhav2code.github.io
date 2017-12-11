---
layout: post
title: Exclude files/folders in tar
---

Here is how to exclude a list of files/folders while tarring 

* create a file with the list of folders/files to exclude 
* example excludelist 

```sh
usr/share/man/*
usr/share/doc/*
usr/share/info/*
usr/local/share/man/*
usr/local/share/info/*
usr/local/share/application/*
usr/lib/locale/locale-archive
usr/lib/jav/*
usr/lib/rpm/*
usr/lib/firmware/*
usr/lib/kbd/keymaps/*
usr/lib/dracut/*
usr/lib/modules/*
var/cache/*
var/lib/rpm/*
var/lib/yum/*
```

* tar czpf temp.tgz -C temp . --exclude-from=excludelist

