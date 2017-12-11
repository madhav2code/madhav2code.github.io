---
layout:     post
title:      "Delete entry from crontab"
subtitle:   "How to delete an entry from crontab."
---

Delete specific entry from crontab.
   
```sh
crontab -l | grep -v 'logrotate' | crontab -
```
   
This would filter out "logroate" from the current entries in crontab


