---
title: "Installing AWS CLI version 2"
date: 2020-04-24T11:16:09-04:00
chapter: false
pre: "<b>7. </b>"
weight: 7
---

- [Click Here](https://awscli.amazonaws.com/AWSCLIV2.pkg) to download and install it.

```bash
$ which aws
/usr/local/bin/aws

$ aws --version
aws-cli/2.0.0 Python/3.7.4 Darwin/19.3.0 botocore/2.0.0dev4
```

- Run the command `aws configure`

```bash
$ aws configure
AWS Access Key ID [None]:
AWS Secret Access Key [None]:
Default region name [None]: ap-southeast-1
Default output format [None]:
```

- Verify `.aws/config` and `.aws/credentials`.

```bash
$ cat .aws/config

$ cat .aws/credentials
```

>**Important**
Congratulations!
Don't forget to record TimeTracker in ClickUp.