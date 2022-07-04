---
layout: post
category: projects
date: 2022-05-10
language: gb
location: The Opensource World
post-title: Mattemost Notify
summary: New release of <i>go-mattermost-notify</i>, a simple and open-source Mattermost notifier written in Go and redistributable under the Apache-2.0 license. You can post <i>text</i> or <i>markdown</i>-formatted messages to a Mattermost channel, via its <i>ID</i>, or send <i>direct messages</i> to a user.
title: Mattemost Notify 1.2.0
---

The version 1.2.0 of the *go-mattermost-notify*,
a simple [Mattermost](https://mattermost.com/) notifier written in Go (golang) and redistributable
under the [Apache-2.0](https://github.com/madrisan/go-mattermost-notify/blob/main/LICENSE) license,
is available for download!

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


### What’s new in this release

#### FIXES

 * Fix all the issues reported by the Go linter.
 * Fix the mispelled mattermost folder in the directory structure :open_mouth:

#### IMPROVEMENTS

 * New command line options `--insecure` for disabling SSL certificate checks (false by default) and `--timeout` (10s by default).
 * Rework and update the `golangci-lint` execution in GitHub Workflows

The source code is available at [GitHub](https://github.com/madrisan/go-mattermost-notify/)
along with the (static) binaries compiled for:

 * [Darwin amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.2.0/darwin_amd64.zip)
 * [FreeBSD amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.2.0/freebsd_amd64.zip)
 * [FreeBSB arm](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.2.0/freebsd_arm.zip)
 * [Linux amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.2.0/linux_amd64.zip)
 * [Linux arm](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.2.0/linux_arm.zip)
 * [Linux arm64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.2.0/linux_arm64.zip)
 * [NetBSD amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.2.0/netbsd_amd64.zip)
 * [OpenBSD amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.2.0/openbsd_amd64.zip)
 * [Windows amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.2.0/windows_amd64.zip)
