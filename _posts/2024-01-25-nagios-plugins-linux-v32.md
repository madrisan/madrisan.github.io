---
layout: post
category: projects
date: 2024-01-25
language: gb
location: The Opensource World
post-title: Nagios Plugins for Linux
summary: Here comes a new release of <i>Nagios Plugins for Linux</i>! This release fixes a Y2038-related issue in <i>check_users</i> and a wrong factor in <i>check_cpufreq</i>, and adds packages for Fedora 39, Linux Alpine 3.18/3.19, and Rocky Linux.
title: Nagios Plugins for Linux v32
---
The version 32 of the Nagios Plugins for Linux ("*Gematria*") is available
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

##### Build

 * *configure*: do not silently ignore missing libcurl and libvarlink.

##### Libraries

 * *lib/netinfo-private*: don't enforce nl_pid.
   Thanks to [Yuri Konotopov (nE0sIghT)](https://github.com/nE0sIghT) for reporting and solving this problem in containerised environments.
 * *lib/netinfo-private*: fix a Clang 17 warning.

##### Plugin check_users

 * *check_users*: fix an issue related to the Y2038 Unix bug.
 * *check_cpufreq*: wrong factor in check_cpufreq for `-G`.
   Thanks to [Grischa Zengel (ggzengel)](https://github.com/ggzengel) for the bug report.

#### ENHANCEMENTS / CHANGES

##### Package creation

 * Add Fedora 39 and drop support for Fedora 36.
 * Add Linux Alpine 3.18 and 3.19 and drop support for Linux Alpine 3.14-3.16.
 * Add Rocky Linux distribution.
 * Fix build of debian packages.

##### GitHub workflows

 * Enable systemd library requirement in the GitHub workflow.
 * Update Linux releases for tests execution in the GitHub workflows.

Full Changelog: [`v31...v32`](https://github.com/madrisan/nagios-plugins-linux/compare/v31..v32)
