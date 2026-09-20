---
layout: post
category: projects
date: 2025-10-06
language: gb
location: The Opensource World
post-title: Open Scores for Piano
summary: An autumn update of <i>Open Scores for Piano</i>, a collection of piano sheet music and transcriptions engraved with LilyPond and distributed with full source code under the CC-BY-NC-SA-4.0 license. This release adds two more Liszt pieces and Margola's <i>Sei sonatine facili</i>, plus new LilyPond 2.25 ornament support.
title: Open Scores for Piano v69
---

The version 69 of *Open Scores for Piano* is available!

Open Scores for Piano is a collection of piano sheet music and piano transcriptions, engraved with
[LilyPond](https://lilypond.org/) and distributed with the full source code, under the
[CC-BY-NC-SA-4.0](https://spdx.org/licenses/CC-BY-NC-SA-4.0.html) license.

<picture>
    <img src="https://media.githubusercontent.com/media/madrisan/open-scores/main/images/open-scores-logo.png"
         class="mx-auto d-block img-fluid pt-3">
</picture>
<p class="text-center pt-2 pb-1">
    <small>
       <a href="https://github.com/madrisan/open-scores">
          <small>Open Scores for Piano</small></a>'s logo
    </small>
</p>

### What’s new in this release

#### ADDED

 * Franz Liszt: Wiegenlied - Chant du berceau S.198
 * Franz Liszt: Zweite Elegie S.197
 * Franco Margola: Sei sonatine facili per pianoforte dc108

#### CHANGED

 * J.S. Bach: Sechs kleine Präludien (BWV 933-938) - use `\atLeft\mordent`.
   LilyPond 2.25 makes it possible to position a mordent to the left side of a note;
   the ugly workaround code used before this feature was available has been removed.
 * J.S. Bach: Suite Anglaise 1 BWV806 - use the new `\bachschleifer` ornament.
   The custom macro `macros-schleifer.ly` has been removed in favor of the new ornament
   available in LilyPond 2.25.

Full Changelog: [`v68...v69`](https://github.com/madrisan/open-scores/compare/v68..v69)

The project and its LilyPond sources are available at [GitHub](https://github.com/madrisan/open-scores),
and the updated PDF scores can be downloaded from the
[v69 release page](https://github.com/madrisan/open-scores/releases/tag/v69).
