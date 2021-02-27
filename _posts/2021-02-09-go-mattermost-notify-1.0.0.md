---
layout: post
title: Mattemost Notify 1.0.0
date: 2021-02-09
language: gb
location: The Opensource World
category: projects
summary: First stable release of <i>go-mattermost-notify</i>, a simple and open-source Mattermost notifier written in Go and redistributable under the Apache-2.0 license. You can post <i>text</i> or <i>markdown</i>-formatted messages to a Mattermost channel (via its <i>ID</i>) or send <i>direct messages</i> to a user.
---

<div class="pb-2">
<h2 class="text-info">Mattemost Notify</h2>
</div>

I'm very proud to announce the immediate release of my last opensource project

<div class="p-3 mb-3 h5 text-center bg-info text-white font-weight-bold shadow">
go-mattermost-notify v1.0.0
</div>

a simple [Mattermost](https://mattermost.com/) notifier written in Go (golang) and redistributable
under the [Apache-2.0](https://github.com/madrisan/go-mattermost-notify/blob/main/LICENSE) license.

<picture>
    <img src="https://raw.githubusercontent.com/madrisan/go-mattermost-notify/main/images/go-mattermost-notify-logo.png"
         class="mx-auto d-block img-fluid pt-3">
</picture>
<p class="text-center pt-2 pb-1">
    <small>
       <a href="https://github.com/madrisan/go-mattermost-notify">
          <small>go-mattermost-notify</small></a>'s logo
    </small>
</p>

This program makes use of the Go libraries *http* and *url* for interacting with a Mattermost
server (via its [REST API v4](https://api.mattermost.com/v4/))
and *[Cobra](https://cobra.dev/)* coupled with *[Viper](https://github.com/spf13/viper)*
to implement the command-line interface.

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

A few settings can be configured also in a *yaml* configuration file.

<picture>
    <img src="https://raw.githubusercontent.com/madrisan/go-mattermost-notify/main/images/mattermost_post_example.png"
         class="mx-auto d-block img-fluid pt-1">
</picture>
<p class="text-center pt-2 pb-31">
    <small>Example of a message posted to Mattermost</small>
</p>

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
