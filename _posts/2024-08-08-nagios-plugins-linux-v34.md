---
layout: post
category: projects
date: 2024-08-08
language: gb
location: The Opensource World
post-title: Nagios Plugins for Linux
summary: A fresh release of <i>Nagios Plugins for Linux</i> has landed! This release adds two new plugins, <i>check_selinux</i> and a <code>-l/--list</code> option for <i>check_ifmount</i>, plus a fix for the Icinga2 <i>check_clock</i> configuration.
title: Nagios Plugins for Linux v34
---
The version 34 of the Nagios Plugins for Linux ("*Heatwaves*") is available
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

 * Missing header `npl_selinux.h` in Makefile (`noinst_HEADERS`).

##### Libraries

 * *lib/container*: docker API versions before v1.24 are deprecated, so 1.24 is set as the minimum version required.
 * *lib/sysfsparser*: fix gcc warning: 'crit_temp' may be used uninitialized.
 * *lib/sysfsparser*: better signature for function `sysfsparser_getvalue`.

##### Contrib (Icinga2)

 * Fix Icinga2 config for *check_clock* by Lorenz Kästle.
   Previously the time reference value was evaluated only during the startup of Icinga 2 and therefore a fixed point in time.
   This change makes it a function which gets evaluated every time the check is executed.

#### ENHANCEMENTS

##### Plugin check_ifmount

 * Add the cmdline switch `-l|--list` to list the mounted filesystems (same output as the *mount* command executed without options).

##### Plugin check_selinux

 * New plugin *check_selinux* that checks if SELinux is enabled.

##### Package creation

 * Add Linux Alpine 3.20 and drop version 3.17.
 * Add Fedora 40, drop Fedora 38.

##### Documentation

 * Fix typo.
 * Add a link to discussion [#147](https://github.com/madrisan/nagios-plugins-linux/discussions/147).
 * Add a note on the Debian package *nagios-plugins-contrib*.

Full Changelog: [`v33...v34`](https://github.com/madrisan/nagios-plugins-linux/compare/v33..v34)
