# How this repository was made (United States (Oregon))

This file is written by the build on 2026-10-30, the day the source data was retrieved.

## Sources

| Source | Address | Retrieved | Licence |
| --- | --- | --- | --- |
| Oregon Legislature, Oregon Revised Statutes and Constitution (Internet Archive captures) | <https://www.oregonlegislature.gov/bills_laws/Pages/ORS.aspx> | 2026-10-30 | Public statute text |

Every word of law in this repository comes from these sources. Lexifina reads them and records each act's dated versions, and the laws that made each change, in one corpus file. This repository is built from that file.

## What is in it

| Act | Title | Versions | Span |
| --- | --- | ---: | --- |
| `constitution` | Constitution of Oregon | 1 | 2026-10-19 to 2026-10-19 |
| `ors-163` | Oregon Revised Statutes, chapter 163: Offenses Against Persons | 1 | 2026-10-22 to 2026-10-22 |
| `ors-164` | Oregon Revised Statutes, chapter 164: Offenses Against Property | 1 | 2026-07-07 to 2026-07-07 |
| `ors-060` | Oregon Revised Statutes, chapter 60: Private Corporations | 1 | 2026-09-23 to 2026-09-23 |
| `ors-093` | Oregon Revised Statutes, chapter 93: Conveyancing and Recording | 1 | 2026-10-24 to 2026-10-24 |

The build made 5 commits:

| Commits | Kind |
| ---: | --- |
| 5 | first version of an act |
| 0 | one law on its in-force day |
| 0 | changes no amendment note explains, credited to the publisher |

Other counts:
- 0 commits on the branch `future`: laws not yet in force on 2026-10-30.
- 0 commits dated 1 January 1970: in force before 1970, with the real day in their `In-force` trailer.
- 5 laws in the record.
- 5 tags.

## Dates

Each commit is dated at noon (America/Los_Angeles) on the day the change took effect. The other dates, enacted and published, are trailers.

When a law gives no date of its own, the default rule applies: No dated history is published: each text is the oldest version available, dated from the day the Internet Archive captured the official page. https://www.oregonlegislature.gov/bills_laws/Pages/ORS.aspx

## How the history is built

`tools/build.py` turns the corpus into this history in one pass: one commit per law, on the day it took effect. The same corpus always gives the same commit hashes. `tools/check_repo.py` reads every version back from git and compares it with the corpus. `tools/on.py` shows the law as it stood on any date. The corpus format is described in `tools/SCHEMA.md`.

- Corpus: sha256 `b8c3388f21c9f80eb9a0f4a48f77ebff296ecbe7b90e5d4308ee8e8310d5cefa` (1281818 bytes).
- Builder blob hashes (`git hash-object`): `build.py` `a4faa25af85facb64b956b372f6b528aafdd7ec1`, `check.py` `3e59cb6f05eccb94a9ec14431a7f6781221e83ef`, `on.py` `644a6c0857fbcc72562032b58d57aa113fee0641`.
- Python 3.12.10; git version 2.46.0.windows.1.

## Checks

Not yet run for this build.

No second build of this corpus has been compared yet.

## Decisions made by hand

- English only. First build: the Constitution and ORS chapters 163 and 164 (criminal), 60 (business corporations) and 93 (conveyancing).
- the archive is the source of the bytes, the Legislature the publisher.
- Each text has one version, "oldest version available", dated from the capture day and credited to the publisher.
- Bracketed history notes at the end of each section, tables of contents and Constitution article indexes are not kept.

## What AI did and did not do

The scripts that read the sources and build this repository were written by Claude Code running Claude Opus 5.5 (`claude-opus-5-5`) under Lexifina's direction.

No model wrote, translated or corrected legal text. No model runs at build time. Every word of law in this repository comes from the official sources above.

The commit messages are written by `build.py` from the source data.

Model use at data-build time:
- none (scripts only; no model wrote or altered legal text)
