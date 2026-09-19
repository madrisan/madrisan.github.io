---
layout: post
category: projects
date: 2026-01-04
language: gb
location: The Opensource World
post-title: Nagios Plugins for Linux
summary: Nagios Plugins for Linux is back with a new release! This release adds an <code>-x/--exclude</code> option to <i>check_readonlyfs</i>, fixes a couple of static-analyzer warnings, and refreshes the supported package distributions.
title: Nagios Plugins for Linux v35
---
The version 35 of the Nagios Plugins for Linux is available for download!

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

 * Fix *configure* on Fedora 42 (missing gawk).

##### Libraries

 * Fix warnings spotted out by scan-build.

##### Plugins

 * *check_memory*: fix warnings reported by clang.

##### Test framework

 * Fix warnings reported by scan-build (clang).

#### ENHANCEMENTS

##### Documentation

 * Tested with gcc 15.0.1 and clang 20.1.3.
 * Add a badge with the total number of downloads.

##### Package creation

 * Add Linux Alpine 3.23, 3.22 and drop version 3.18, 3.19, 3.20.
 * Add Debian 13, drop Debian 10.
 * Add Fedora 41, 42 and 43, drop Fedora 38, 39, and 40.

##### Plugin check_readonlyfs

 * New option `-x/--exclude` to check all but the file systems passed as arguments.
   Feature asked by [Michael Wolf (michaeldcwolf)](https://github.com/michaeldcwolf).

Full Changelog: [`v34...v35`](https://github.com/madrisan/nagios-plugins-linux/compare/v34..v35)
