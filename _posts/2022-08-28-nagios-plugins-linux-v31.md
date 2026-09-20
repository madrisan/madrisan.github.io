---
layout: post
category: projects
date: 2022-08-28
language: gb
location: The Opensource World
post-title: Nagios Plugins for Linux
summary: Nagios Plugins for Linux keeps growing, and a new release is available! This release adds a brand new plugin <i>check_filecount</i>, new units support for <i>check_memory</i>, and Icinga2 command configurations contributed by the community.
title: Nagios Plugins for Linux v31
---
The version 31 of the Nagios Plugins for Linux ("*Counter-intuitive*") is available
for download!

The Nagios Plugins for Linux is a
[free](https://github.com/madrisan/nagios-plugins-linux/blob/master/COPYING)
and open source set of Nagios and Icinga plugins for monitoring the major system parameters of a
Linux server. The source code is available at
[GitHub](https://github.com/madrisan/nagios-plugins-linux/releases/).
You can find the documentation in the project
[main page](https://github.com/madrisan/nagios-plugins-linux) or the associated
[wiki](https://github.com/madrisan/nagios-plugins-linux/wiki) site.

### What’s new in this release

#### FIXES

##### Libraries

 * *lib/container_docker_memory*: fix an issue reported by clang-analyzer.
 * Make sure *sysfs* is mounted in the plugins that require it.

#### ENHANCEMENTS / CHANGES

##### Plugin check_filecount

 * New plugin *check_filecount* that returns the number of files found in one or more directories.

##### Plugin check_memory

 * Support new units kiB/MiB/GiB.
   Feature asked by [mdicss](https://github.com/mdicss).
   See the discussion [#120](https://github.com/madrisan/nagios-plugins-linux/discussions/120).

##### contrib/icinga2/CheckCommands.conf

 * Contribution from Lorenz [RincewindsHat](https://github.com/RincewindsHat): add icinga2 command configurations.

##### Build

 * *configure*: ensure libprocps is v4.0.0 or better if the experimental option `--enable-libprocps` is passed to `configure`.

##### Test framework

 * Add some unit tests for *lib/xstrton*.
 * New unit tests `tslibfiles_{filecount,hiddenfile,size}`.

##### Package creation

 * Add Linux Alpine 3.16 and remove version 3.13.
 * Do not package experimental plugins in the rpm *nagios-plugins-linux-all*.
 * Add Fedora 36 and drop Fedora 33 support.
 * CentOS 8 died a premature death at the end of 2021. Add packages for CentOS Stream 8 and 9.

##### GitHub workflows

 * Build the Nagios Plugins Linux on the LTS Ubuntu versions only.
 * Add build tests for all the supported oses, and a CodeQL analysis.
 * CentOS 8 died a premature death at the end of 2021. Remove it from the list of test oses.

Full Changelog: [`v30...v31`](https://github.com/madrisan/nagios-plugins-linux/compare/v30..v31)
