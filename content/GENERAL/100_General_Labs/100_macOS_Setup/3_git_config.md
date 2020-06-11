---
title: "git config"
date: 2020-04-24T11:16:09-04:00
chapter: false
pre: "<b>3. </b>"
weight: 3
---

#### git config

>**Reference -**
https://uw-madison-aci.github.io/git-novice/02-setup/

```bash
$ git config --global user.name "Sai Linn Thu"
$ git config --global user.email "sai.grincerlabs@gmail.com"
$ cat .gitconfig
[user]
	name = Sai Linn Thu
	email = sai.grincerlabs@gmail.com

$ git config --global color.ui "auto"

$ git config --global core.editor "code --wait" #VS Code
```

Check your settings at any time:
```bash
$ git config --list
credential.helper=osxkeychain
user.name=Sai Linn Thu
user.email=sai.grincerlabs@gmail.com
color.ui=auto
core.editor=code --wait
```

