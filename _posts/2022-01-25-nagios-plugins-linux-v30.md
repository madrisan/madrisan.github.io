---
layout: post
category: projects
date: 2022-01-25
language: gb
location: The Opensource World
post-title: Nagios Plugins for Linux
summary: This <i>Nagios Plugins for Linux</i> contains a complete set of enterprise ready Nagios-compatible Plugins for monitoring Linux hosts. This new version contains fixes for the plugin <i>check_pressure</i> and the Debian multi-packages build.
title: Nagios Plugins for Linux v30
---
The version 30 of the Nagios Plugins for Linux ("*Low Pressure*") is available
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

##### Plugin check_pressure

 * Display values per second regardless of the delay, and ensure the delta of "some" is calculated correctly.
 * Thanks to [Christian Bryn (epleterte)](https://github.com/epleterte) for reporting and fixing a typo in the git clone command.

##### Package creation

 * Fix Debian packages creation.

#### ENHANCEMENTS / CHANGES

##### Libraries

 * *lib/netinfo*: fix a LGTM static analyzer alert.

##### Packages

Release updates:

 * Add Debian 11 and drop Debian 8,
 * Add Fedora 35 and drop Fedora 32,
 * Add Linux Alpine 3.15 and drop version 3.12.
