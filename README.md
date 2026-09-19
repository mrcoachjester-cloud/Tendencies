# Tendencies Analyzer

This repository contains the football tendencies analyzer built around the supplied Hudl/Google Sheets play-data schema.

## Core fields
- GN/LS: gain/loss
- OFF FORM: formation
- PERSONNEL: personnel
- MOTION: motion
- DN / DIST: down and distance
- YARD LN: field position
- HASH: hash
- AWAY: away/team context
- PLAY DIR / PLAY (STR/WK): direction and strength/weakness
- SCHEME: scheme
- OFF PLAY: offensive play
- PASS PRO: protection
- READ: read
- PS / WS / STUD: alignment
- COMMENTS: comments

## Explosives
- Run: GN/LS >= 15
- Pass: GN/LS >= 20
- Scrambles are treated as QB rushing when identified by the source data.

## Situational analysis
The analyzer will report combinations including down/distance, 1st & 10, 2nd & 5-7, 3rd & short, backed up, plus territory, red zone, coming out, field/boundary, left/right, hash + formation, formation + motion, and formation + personnel.

## Sequence analysis
For each explosive play, preceding play(s) are examined and compared with the overall sample. Counts and rates are reported so recurring sequences can be identified without treating repetition alone as proof of a meaningful tendency.

The analyzer uses the supplied field names rather than inventing alternate schema.
