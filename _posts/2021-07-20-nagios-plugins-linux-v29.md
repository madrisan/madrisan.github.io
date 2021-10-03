---
layout: post
category: projects
date: 2021-07-20
language: gb
location: The Opensource World
post-title: Nagios Plugins for Linux
redirect_from:
 - /blog/2021/07/20/nagios-plugins-linux-v29
summary: A new version of <i>Nagios Plugins for Linux</i> is out! This project contains a quite complete set of enterprise ready Nagios-compatible Plugins for monitoring Linux hosts. In this release the plugin <i>check_temperature</i> has been improved and a modular Debian multi-packages build is now available.
title: Nagios Plugins for Linux v29
---
The version 29 of the Nagios Plugins for Linux ("*High Temperatures*") is available
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

##### FIXES

###### Plugin check_temperature

 * Do not display thermal ranges if `-t|--thermal_zone` in not set at command-line.

##### ENHANCEMENTS

###### Plugin check_temperature

 * Improve the output message by adding the thermal device when available;
 * List also the devices that display a temperature of 0°C to be more consistent with the tool 'sensors';
 * Improve the help message;
 * New command-line option `-l|--list` for displyaing the all the thermal sensors reported by the kernel.

###### Package creation

 * Update the list of supported platforms by adding Alpine 3.13 and 3.14 and Fedora 34;
 * Several improvements to the Debian packaging (thanks to [Vincent Olivert-Riera](https://github.com/vincent-olivert-riera) for the PR);
 * Build Debian multi-packages instead of a single package providing all binary plugins.
   This will permit these plugins to cohexist with the Nagios native ones.

###### Test framework

 * Switch to the latest stable OSes in GitHub workflow.

###### Documentation

 * Update the documentation for linking against procps-ng newlib;
 * Thanks to [Christian Bryn (epleterte)](https://github.com/epleterte) for reporting and fixing a typo in the git clone command.

