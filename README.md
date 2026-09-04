# PgnTours

An archive of chess tournaments in PGN form, with crosstables.

Every ZIP is generated from the corresponding
[CTML](https://github.com/ianrastall/ctml) source in
`ctml/tours/*.ctml`, so the moves, players, and metadata all come from
one machine-verified record of the event.

## Layout

Files live in decade folders (`1850s/`, `1880s/`, …). Each ZIP contains
two files:

- `YYYYMMDD-YYYYMMDD-slug.pgn` — one game per PGN block, SAN moves
  converted from CTML's UCI, headers pulled from the CTML metadata.
- `YYYYMMDD-YYYYMMDD-slug.html` — self-contained crosstable with
  standings and per-round game list.

The filename slug is the CTML basename with the underscore between the
date pair and the event slug replaced by a hyphen, so
`20260525-20260605_14th-norway-chess.ctml` becomes
`20260525-20260605-14th-norway-chess.zip`.

## Browsing

The [Chess Nerd Tournament Archive
page](https://chessnerd.net/tournament-archive.html) is a searchable
table over these ZIPs with dates, place, cadence, format, and game
counts.
