---
layout: post
title: How to change password in chroot using script
---

Script to Change password in chroot

```sh
#!/bin/bash

sudo chroot ramfs /bin/bash -x <<'EOF'
echo "mypassword" | passwd root --stdin
exit 0
EOF
```
