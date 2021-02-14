---
layout: post
title: Mattemost Notify 1.0.0
date: 2021-02-09
language: gb
location: The Opensource World
category: projects
summary: First stable release of go-mattermost-notify, a simple Mattermost notifier written in Go.
---

I'm very proud to announce the immediate release of

<div class="p-3 mb-2 h5 text-center font-weight-bold bg-info text-white">
go-mattermost-notify v1.0.0
</div>

a simple [Mattermost](https://mattermost.com/) notifier written in Go (golang) and redistributable
under the [Apache-2.0](https://github.com/madrisan/go-mattermost-notify/blob/main/LICENSE)
opensource license.

This program makes use of the Go libraries *http* and *url* for interacting with a Mattermost
server and *[Cobra](https://cobra.dev/)* coupled with *[Viper](https://github.com/spf13/viper)*
to implement the command-line interface.

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

<picture>
    <img src="https://raw.githubusercontent.com/madrisan/go-mattermost-notify/main/images/mattermost_post_example.png"
         class="mx-auto d-block img-fluid pt-3">
</picture>
<p class="text-center pt-2 pb-31">
    <small>Example of a post message</small>
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
