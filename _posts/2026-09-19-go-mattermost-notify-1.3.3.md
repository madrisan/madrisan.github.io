---
layout: post
category: projects
date: 2026-09-19
language: gb
location: The Opensource World
post-title: Mattemost Notify
summary: A security-hardening release of <i>go-mattermost-notify</i>, a simple and open-source Mattermost notifier written in Go and redistributable under the Apache-2.0 license. You can post <i>text</i> or <i>markdown</i>-formatted messages to a Mattermost channel, via its <i>ID</i>, or send <i>direct messages</i> to a user.
title: Mattemost Notify 1.3.3
---

The version 1.3.3 of the *go-mattermost-notify*,
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

#### SECURITY FIXES

 * `github.com/go-viper/mapstructure/v2`: may leak sensitive information in logs when processing malformed data.
   Affected versions: `github.com/go-viper/mapstructure/v2` < 2.3.0. Fix: 2.5.0.
   See: [GO-2025-3787](https://pkg.go.dev/vuln/GO-2025-3787).
 * Update `golang.org/x/text` and `golang.org/x/sys` to their latest patched releases, addressing
   further advisories reported against modules required by the project.

#### IMPROVEMENTS

 * Add a Trivy vulnerability scan to the GitHub Workflows, with results published to the GitHub
   Security tab.
 * Update the Go compiler and the `golangci-lint` version used in the build scripts.
 * Update GitHub Actions (`setup-go`, `checkout`, `golangci-lint-action`, `codeql-action/upload-sarif`,
   `trivy-action`) to versions that no longer run on deprecated Node.js runtimes, and address the
   upcoming CodeQL v3 deprecation.
 * Drop `github.com/golangci/golangci-lint` and `github.com/mitchellh/gox` from `go.mod`: they had been
   pulled in as real module requirements by `make bootstrap`'s use of `go get -u` instead of
   `go install`, even though neither is imported by this module's code.
 * Migrate to `golangci-lint` v2 and `golangci-lint-action` v9 (the last `golangci-lint-action` release
   supporting v1.x only ships a Node 20 runtime, which GitHub is deprecating). Add a minimal
   `.golangci.yml` declaring the v2 config schema.

#### BUG FIXES

 * Check a handful of previously-ignored error return values (`mattermost.PrettyPrint`,
   `response.Body.Close`, `fmt.Fprintln`), surfaced by `golangci-lint` v2's default ruleset.
 * Lowercase an error string per Go convention (ST1005).

Full Changelog: [`v1.3.2...v1.3.3`](https://github.com/madrisan/go-mattermost-notify/compare/v1.3.2..v1.3.3)

The source code is available at [GitHub](https://github.com/madrisan/go-mattermost-notify/).
