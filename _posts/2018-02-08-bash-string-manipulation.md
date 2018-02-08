---
layout: post
title: BASH string manipulation
---

### BASH cut last character ###
```sh
str="test"
echo "${str}"
test
str="${str::-1}"
echo "${str}"
tes
```