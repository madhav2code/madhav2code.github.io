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

### BASH check if string starts with ###
```sh
str="test string main"
echo "${str}"
test string main
if [[ "${str}" =~ ^test.* ]]; then
	echo "Yes"
else
	echo "No"
fi
Yes
```

### BASH check if string does not start with ###
```sh
str="test string main"
echo "${str}"
test string main
if [[ ! "${str}" =~ ^test.* ]]; then
	echo "Yes"
else
	echo "No"
fi
No
```