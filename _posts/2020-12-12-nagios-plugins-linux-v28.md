---
layout: post
category: projects
date: 2020-12-12
language: gb
location: The Opensource World
post-title: Nagios Plugins for Linux
summary: A new version of <i>Nagios Plugins for Linux</i> is out! This project contains a quite complete set of enterprise ready Nagios plugins for monitoring Linux boxes. New features include the new plugin <i>check_pressure</i> (that reports the Linux Pressure Stall Information (PSI) exported by Linux kernels 4.20+) and the porting to <i>Linux Alpine</i> 3.12 with packaging available.
title: Nagios Plugins for Linux v28
---
The version 28 of the Nagios Plugins for Linux ("*Alpine Hike*") is available
for download!

The Nagios Plugins for Linux is a
[free](https://github.com/madrisan/nagios-plugins-linux/blob/master/COPYING)
and open source set of Nagios and Icinga plugins for monitoring the major system parameters of a
Linux server. The source code is available at
[GitHub](https://github.com/madrisan/nagios-plugins-linux/releases/).
You can find the documentation in the project
[main page](https://github.com/madrisan/nagios-plugins-linux) or the associated
[wiki](https://github.com/madrisan/nagios-plugins-linux/wiki) site.

#### What’s new in this release

###### Fixes

A few Clang and GCC warnings have been fixed.

###### Enhancements

New plugin *check_pressure* that reports the Linux Pressure Stall Information (PSI)
exported by Linux kernels 4.20+ (in the `/proc/pressure/` folder).

```bash
check_pressure --cpu  # return the cpu pressure metrics
check_pressure --io  # return the io (block layer/filesystems) pressure metrics
check_pressure --memory  # return the memory pressure metrics
```

###### Build system

Here are some notable news:

 * Integrate *Nagios Plugins for Linux* with *GitHub Workflow* tests;
 * Add [Linux Alpine](https://alpinelinux.org/) and [Ubuntu](https://ubuntu.com/)
   to the list of supported and automatically tested Linux distributions;
 * Update the list of supported platforms by adding Alpine 3.12 and Fedora 33;
 * Make the `packages/docker-shell-helpers` folder a git
   [submodule](https://github.com/madrisan/docker-shell-helpers).

###### Package creation

A Linux Alpine (3.12) native package can be now created by running the command

```bash
make -C packages alpine-3.12
```
