---
title: "Setting up bash"
date: 2020-04-24T11:16:09-04:00
chapter: false
pre: "<b>5. </b>"
weight: 5
---

- Verify the current `bash` version and location.
```bash
$ which bash
/bin/bash

$ echo $BASH_VERSION
3.2.57(1)-release
```

- Install bash using Homebrew. The packages will be installed under `/usr/local/Cellar`
```bash
$ brew install bash
$ which bash
/usr/local/bin/bash
```

- As a result of that, we now have two version of `bash`.
```bash
$ which -a bash
/usr/local/bin/bash
/bin/bash
```

- We will be using our new version of `bash`.
```bash
$ which bash
/usr/local/bin/bash

$ bash --version
GNU bash, version 5.0.16(1)-release (x86_64-apple-darwin19.3.0)
Copyright (C) 2019 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>

This is free software; you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.
```