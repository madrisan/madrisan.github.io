---
layout: post
category: projects
date: 2024-04-01
language: gb
location: The Opensource World
post-title: Nagios Plugins for Linux
summary: Nagios Plugins for Linux has just been updated! This release brings the same fixes as v32 (Y2038 issue in <i>check_users</i>, wrong factor in <i>check_cpufreq</i>) plus fixes for two test suites on 32-bit architectures.
title: Nagios Plugins for Linux v33
---
The version 33 of the Nagios Plugins for Linux ("*Śmigus-Dyngus*") is available
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

##### Tests

 * Fix tests `tslibxstrton_sizetollint` and `tslibpressure` on 32-bit architectures.

#### ENHANCEMENTS / CHANGES

##### Package creation

 * Add Fedora 39 and drop support for Fedora 36.
 * Add Linux Alpine 3.18 and 3.19 and drop support for Linux Alpine 3.14-3.16.
 * Add Rocky Linux distribution.
 * Fix build of debian packages.

##### GitHub workflows

 * Enable systemd library requirement in the GitHub workflow.
 * Update Linux releases for tests execution in the GitHub workflows.

Full Changelog: [`v32...v33`](https://github.com/madrisan/nagios-plugins-linux/compare/v32..v33)
