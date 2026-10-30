# United States (Oregon): law history in git

A first build of Oregon law as git: one file per provision, with the text published by the Oregon Legislature (Legislative Counsel) ([oregonlegislature.gov](https://www.oregonlegislature.gov/bills_laws/Pages/ORS.aspx)). It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `united-states/oregon/`. Language: English.

**What is in it now**

| Folder | Law | Versions | History |
| --- | --- | ---: | --- |
| `constitution/` | Constitution of Oregon (1857, as amended) | 1 | Oldest version available (retrieved 2026-07-07 to 2026-10-24 (the Internet Archive capture day of each page)) |
| `ors-163/` | ORS chapter 163: Offenses Against Persons | 1 | Oldest version available (retrieved 2026-07-07 to 2026-10-24 (the Internet Archive capture day of each page)) |
| `ors-164/` | ORS chapter 164: Offenses Against Property | 1 | Oldest version available (retrieved 2026-07-07 to 2026-10-24 (the Internet Archive capture day of each page)) |
| `ors-060/` | ORS chapter 60: Private Corporations | 1 | Oldest version available (retrieved 2026-07-07 to 2026-10-24 (the Internet Archive capture day of each page)) |
| `ors-093/` | ORS chapter 93: Conveyancing and Recording | 1 | Oldest version available (retrieved 2026-07-07 to 2026-10-24 (the Internet Archive capture day of each page)) |

## What it does not show

Each text therefore has one commit, "oldest version available", credited to the publisher and dated by the retrieval day.
- **Other law.** The rest of the Oregon Revised Statutes is not yet included.
- **Notes.** Source notes, histories and annotations are not law text and are not in the files.

## How it is checked

Every version names its source and the sha256 of the data it was read from. Each version is read back from git and must match `corpus.json` (`tools/check_repo.py`); the results are in `REPRODUCE.md`.

## Sources

| Source | Kind | Past versions | Licence |
| --- | --- | --- | --- |
| [the Oregon Legislature (Legislative Counsel)](https://www.oregonlegislature.gov/bills_laws/Pages/ORS.aspx) | Official publisher | no | Statute text is not copyrightable (Georgia v. Public.Resource.Org, 2020) |

## Licence

See `LICENSE`. This repository is not legal advice and not an official publication.
