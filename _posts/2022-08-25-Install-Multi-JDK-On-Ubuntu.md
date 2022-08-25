---
title: "Install Multi JDK on Ubuntu 20.04"
date: 2022-08-25
tags:
- App
- Ubuntu
---

> ref :https://petewan.com/blog-post/install-and-manage-multiple-java-jdk-and-jre-versions-on-ubuntu-20-04/

## Install mult JDK versions

Check JDK version
`java --version` or `java -version`

Install Jave 11 JDK
```bash
sudo apt install default-jdk
```

Check JDK version
`java --version`

The return result

```
openjdk version "11.0.16" 2022-07.19
OpenJDK Runtime Environment (build 11.016+8-post-Ubuntu-0ubuntu120.04)
OpenJDK 64-Bit Server VM (build 11.016+8-post-Ubuntu-0ubuntu120.04, mixed mode, sharing)
```

Install Jave 8 JDK:
```bash
sudo apt install openjdk-8-jdk
```

## Manage Installed JDK versions

```bash
sudo update-alternatives --config java
```
There will be a interactive respond, choose the target version by hints.
