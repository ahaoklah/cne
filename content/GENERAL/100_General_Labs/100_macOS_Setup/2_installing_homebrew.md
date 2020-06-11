---
title: "Installing Homebrew"
date: 2020-04-24T11:16:09-04:00
chapter: false
weight: 2
pre: "<b>2. </b>"
---

#### Install [Homebrew](https://brew.sh/)

```bash
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew doctor
```

#### Install Homebrew Packages

The packages will be installed under **/usr/local/Cellar** and you can verify as **ls -la /usr/local/Cellar**

```bash
$ brew install wget
$ brew install curl
```

