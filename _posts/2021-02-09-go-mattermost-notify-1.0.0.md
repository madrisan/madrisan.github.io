---
layout: post
title: Mattemost Notify version 1.0.0
date: 2021-02-09
language: gb
location: The Opensource World
category: projects
summary: First stable release of go-mattermost-notify, a simple Mattermost notifier written in Go.
---

I'm very proud to announce the immediate release of *go-mattermost-notify* version 1.0.0,
a simple [Mattermost](https://mattermost.com/) notifier written in Go (golang).

<picture>
    <img src="https://raw.githubusercontent.com/madrisan/go-mattermost-notify/main/images/go-mattermost-notify-logo.png"
         class="mx-auto d-block img-fluid pt-3">
</picture>
<p class="text-center pt-3 pb-3">
    <small>
       Logo &mdash;
       <a href="https://github.com/madrisan/go-mattermost-notify">
          <small>GitHub site</small></a>
    </small>
</p>

You can post *text* or *markdown*-formatted messages to a Mattermost channel (via its *ID*):
```bash
go-mattermost-notify post -c rybfbdi9ojy8xxxjjxc88kh3me -A CI -t "Job Status" -m "The job \#BEEF has failed :bug:" -l critical
```
or send *direct messages* to a user:
```bash
go-mattermost-notify post -c @alice -A CI -t "Job Status" -m "The job \#BEEF ended successfully :tada:" -l success
```
as explained in the
[documentation](https://github.com/madrisan/go-mattermost-notify/blob/main/README.md).

The source code is available at [GitHub](https://github.com/madrisan/go-mattermost-notify/)
along with the (static) binaries compiled for:

 * [Darwin amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.0.0/darwin_amd64.zip)
 * [FreeBSD amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.0.0/freebsd_amd64.zip)
 * [FreeBSB arm](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.0.0/freebsd_arm.zip)
 * [Linux amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.0.0/linux_amd64.zip)
 * [Linux arm](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.0.0/linux_arm.zip)
 * [Linux arm64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.0.0/linux_arm64.zip)
 * [NetBSD amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.0.0/netbsd_amd64.zip)
 * [OpenBSD amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.0.0/openbsd_amd64.zip)
 * [Windows amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.0.0/windows_amd64.zip)
