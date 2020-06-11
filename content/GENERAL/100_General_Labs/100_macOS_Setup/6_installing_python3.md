---
title: "Installing Python3"
date: 2020-04-24T11:16:09-04:00
chapter: false
pre: "<b>6. </b>"
weight: 6
---

#### Installing Python3
>**NOTE -**
**DO NOT INSTALL** `python3` using `Homebrew`, which has a bug in `distutils`. **NOT RECOMMENDED** to symlink `'python'` to `'python3'` binaries as this would cause problems with macOSX and other softwares instead. **CALL python3** directly whenever you want to use it.

- Download and Install python3 from [https://www.python.org/downloads/](https://www.python.org/downloads/)
- Verify as below.
```bash
$ which python3
/Library/Frameworks/Python.framework/Versions/3.8/bin/python3

$ python3 --version
Python 3.8.1
```

- Verify the `.bash_profile`
```bash
$ cat .bash_profile

# Setting PATH for Python 3.8
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.8/bin:${PATH}"
export PATH
```

#### Installing pip3 on macOS
- Run the command as below.
```bash
$ curl -O https://bootstrap.pypa.io/get-pip.py
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 1764k  100 1764k    0     0  5414k      0 --:--:-- --:--:-- --:--:-- 5430k
```

- Install by running `sudo python3 get-pip.py`
```bash
$ sudo python3 get-pip.py
Password:
WARNING: The directory '/Users/sai/Library/Caches/pip' or its parent directory is not owned or is not writable by the current user. The cache has been disabled. Check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
Collecting pip
  Downloading pip-20.0.2-py2.py3-none-any.whl (1.4 MB)
     |████████████████████████████████| 1.4 MB 3.0 MB/s
Collecting wheel
  Downloading wheel-0.34.2-py2.py3-none-any.whl (26 kB)
Installing collected packages: pip, wheel
  Attempting uninstall: pip
    Found existing installation: pip 19.2.3
    Uninstalling pip-19.2.3:
      Successfully uninstalled pip-19.2.3
Successfully installed pip-20.0.2 wheel-0.34.2
```
- Verify as below.
```bash
$ which pip
/Library/Frameworks/Python.framework/Versions/3.8/bin/pip

$ which pip3
/Library/Frameworks/Python.framework/Versions/3.8/bin/pip3


$ pip3 list
Package    Version
---------- -------
pip        20.0.2
setuptools 41.2.0
wheel      0.34.2
```