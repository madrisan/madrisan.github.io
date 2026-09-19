---
layout: post
category: projects
date: 2025-03-21
language: gb
location: The Opensource World
post-title: Mattemost Notify
summary: Right on the heels of that, a further update of <i>go-mattermost-notify</i>, a simple and open-source Mattermost notifier written in Go and redistributable under the Apache-2.0 license. You can post <i>text</i> or <i>markdown</i>-formatted messages to a Mattermost channel, via its <i>ID</i>, or send <i>direct messages</i> to a user.
title: Mattemost Notify 1.3.2
---

The version 1.3.2 of the *go-mattermost-notify*,
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

 * Fix SA1019: `io/ioutil` has been deprecated since Go 1.19: as of Go 1.16, the same functionality
   is now provided by package `io` or package `os`, and those implementations should be preferred
   in new code.
 * Fix some GitHub workflows issues.

Full Changelog: [`v1.3.1...v1.3.2`](https://github.com/madrisan/go-mattermost-notify/compare/v1.3.1..v1.3.2)

The source code is available at [GitHub](https://github.com/madrisan/go-mattermost-notify/)
along with the (static) binaries compiled for:

 * [Darwin amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/darwin_amd64.zip)
 * [FreeBSD amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/freebsd_amd64.zip)
 * [FreeBSB arm](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/freebsd_arm.zip)
 * [Linux amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/linux_amd64.zip)
 * [Linux arm](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/linux_arm.zip)
 * [Linux arm64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/linux_arm64.zip)
 * [NetBSD amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/netbsd_amd64.zip)
 * [OpenBSD amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/openbsd_amd64.zip)
 * [Solaris amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/solaris_amd64.zip)
 * [Windows amd64](https://github.com/madrisan/go-mattermost-notify/releases/download/v1.3.2/windows_amd64.zip)
