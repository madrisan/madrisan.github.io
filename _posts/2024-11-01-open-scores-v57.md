---
layout: post
category: projects
date: 2024-11-01
language: gb
location: The Opensource World
post-title: Open Scores for Piano
summary: A new release of <i>Open Scores for Piano</i>, a collection of piano sheet music and transcriptions engraved with LilyPond and distributed with full source code under the CC-BY-NC-SA-4.0 license. This release adds three more preludes and fugues from Bach's <i>Das wohltemperierte Klavier</i> and Chopin's <i>Valse</i> from the Morgan Library manuscript.
title: Open Scores for Piano v57
---

The version 57 of *Open Scores for Piano* is available!

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

 * J.S. Bach: Das wohltemperierte Klavier – Erster Teil: Praeludium und Fuga VI
 * J.S. Bach: Das wohltemperierte Klavier – Erster Teil: Praeludium und Fuga VII
 * J.S. Bach: Das wohltemperierte Klavier – Erster Teil: Praeludium und Fuga VIII
 * J.S. Bach: Das wohltemperierte Klavier – Erster Teil: add J.S. Bach manuscript
 * Frédérich Chopin: Valse (Morgan Library & Museum Manuscript 2024)

#### CHANGED

 * J.S. Bach: Das wohltemperierte Klavier – number of voices of the fugues as in Bach's manuscript
 * J.S. Bach: Die Kunst der Fuge (BWV1080) - automatic page number in the index using `\page-ref`
 * J.S. Bach: Die Kunst der Fuge (BWV1080) - use a dashed-line as VoiceFollower style

#### FIXED

 * J.S. Bach: Die Kunst der Fuge (BWV1080) - fix some "too many colliding rests" warnings
 * Ludwig van Beethoven: Klaviersonate Nr.8 c-moll Opus 13 - fixes

Full Changelog: [`v56...v57`](https://github.com/madrisan/open-scores/compare/v56..v57)

The project and its LilyPond sources are available at [GitHub](https://github.com/madrisan/open-scores),
and the updated PDF scores can be downloaded from the
[v57 release page](https://github.com/madrisan/open-scores/releases/tag/v57).
