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

### BASH get last character ###
```sh
str="test"
echo "${str}"
test
str="${str: -1}"
echo "${str}"
t
```

### BASH replace white space with underscore (_) in string ###
```sh
str="test string main"
echo "${str}"
test string main
str="${str// /_}"
echo "${str}"
test_string_main
```