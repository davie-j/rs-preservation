# rs-preservation

AI slop README. I aint writing all that

Screenshots, quest scrolls and interface images of Jagex's RuneScape from 2002 to 2007, recovered from the
Internet Archive's Wayback Machine (fansites, forum threads, image hosts and players' personal home pages) and from
early YouTube uploads.

Only the real game is here. Fakes, parodies, edited images, fan art and private-server screenshots were sorted out
and are not part of this repository. Every file has a row in the `SOURCES.csv` of its folder, with the original URL,
the Wayback Machine link, the original file date and a SHA-1.

## Layout

| Folder | Files | What it holds |
|---|---:|---|
| `quest-completion/<Quest>/` | 447 | Quest-completion scrolls, one folder per quest (126 quests), plus a few real in-quest message scrolls |
| `screenshots/2003 … 2007/` | 2,065 | RuneScape 2 client screenshots, by year of the original file (2003 is the December 2003 members beta) |
| `screenshots/runescape-classic/` | 16 | RuneScape Classic screenshots (2002–2005) |
| `other-interfaces/` | 437 | Crops: dialogue, shops, level-ups, trade and duel windows, bank, stats, maps, items |
| `jagex-official-media/` | 52 | Jagex's own material: the runescape.com screenshot gallery, website pages, logo, support e-mails, a wallpaper |
| `videos/` | 2 | 2004 player recordings: a RuneScape Classic Wilderness fight and a clan promo |

## Pictures per year

3,017 pictures (plus 2 videos), counted by the year of each file's original date.

| Year | Screenshots | Quest scrolls | Interfaces & crops | Jagex media | **Total** |
|---|---:|---:|---:|---:|---:|
| 2002 | 3 | – | – | – | **3** |
| 2003 | 25 | 2 | 1 | – | **28** |
| 2004 | 1,102 | 71 | 206 | 10 | **1,389** |
| 2005 | 538 | 225 | 180 | 40 | **983** |
| 2006 | 380 | 132 | 46 | 2 | **560** |
| 2007 | 33 | 4 | 4 | – | **41** |
| 2008 | – | 11 | – | – | **11** |
| 2009 | – | 2 | – | – | **2** |
| **Total** | **2,081** | **447** | **437** | **52** | **3,017** |

The screenshot column includes the 16 RuneScape Classic screenshots under their own years. The 2008–2009 quest scrolls
are YouTube frames dated by upload and one Zybez guide image dated by a site migration; they show 2006-and-later
scrolls. Some RuneHQ and Sal's Realm images carry those sites' 2005 migration dates (see the note at the end).

## What counts as the real game

Every image was checked by eye. Where that was not enough, the page it was posted on decided (the forum thread
title or the folder name on the original site). Images were left out when they:
- came from a private server: invented quests (such as "Green Beret"), more quest points than existed at the time,
  NPCs Jagex never made, moderator tools in a player's menus, or a private-server client in the window title;
- came from a modern recreation (2004Scape, Scape05), however close they look to the 2004 game;
- were edited by a player: posted in a "fakes" thread or a fakes folder, invented game messages, pasted-in objects,
  or mockups made for fan suggestion threads.

Kept on purpose: Hazeel Cult's "You have… kind of… completed" scroll is Jagex's own joke inside the real quest;
Regicide's message scrolls are real quest scrolls; real screenshots that a player only circled or labelled are kept,
with a note in `SOURCES.csv`.

## The target scrolls

The project's main goal is the original 2004 ("old-style") completion scrolls of nine quests.

| Quest | Original 2004 scroll | In the collection |
|---|---|---|
| Underground Pass | **Found** | 24 Apr 2004, full client, Total Points 98 (Finnish player's home page, koti.mbnet.fi) |
| Scorpion Catcher | **Found** | 22 May 2004, full client, Total Points 100 (koti.mbnet.fi) |
| Tribal Totem | **Found** | 15 Jul 2004 full size (exs.cx), 12 Jul 2004 small (Romanian fansite) |
| Hazeel Cult | Found, side unknown | Sal's Realm guide scroll, Total Points 92; the wanted evil-side scroll is not confirmed |
| Temple of Ikov | Wrong side only | Old-style scroll for Armadyl; the wanted Lucien side exists only in a 2007–09 design |
| Regicide | Not found | 2004 start-of-quest message scroll (22 Sep 2004) and 2005–06 new-style scrolls |
| Fight Arena | Not found | 2005 new-style scrolls only |
| Monk's Friend | Not found | 2005 new-style scroll and a 2008 YouTube frame |
| Druidic Ritual | Not found | 2006 new-style scrolls (RuneHQ and a July 2006 YouTube frame) and a 2008 YouTube frame |

## SOURCES.csv

One per top-level folder; `file` is the path below that folder.

| Column | Meaning |
|---|---|
| `file` | path of the file below the folder |
| `category` | official game: quest scroll, screenshot, interface or crop, Jagex material, or video |
| `description` | what the image shows |
| `quest`, `version` | quest scrolls only: quest name and scroll design (old-style 2004, new-style 2005+, message scroll) |
| `original_file_date` | the server's last-modified date for the file, or the capture / upload date when there was none |
| `wayback_capture`, `original_url`, `wayback_url` | where it was recovered from |
| `source_page` | the archived forum thread or page that embedded it, when known |
| `bytes`, `sha1` | size and hash of the file as recovered |
| `note` | provenance remarks |
| `previous_file` | an earlier file name, where a file was renamed |

Some dates are site migration dates rather than the date the screenshot was taken: Sal's Realm (18 Nov 2005,
3 Dec 2006), RuneHQ (19 Oct 2005) and Zybez (14 Oct 2009). YouTube frames carry the upload date.
