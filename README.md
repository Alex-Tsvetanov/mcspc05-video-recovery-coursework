# mcspc05-video-recovery-coursework

Course work for MCSPC05, *Видео и аудио анализ в криминалистиката* (Video and Audio
Analysis in Forensics), MEng Cybersecurity and Cybercrime Prevention, Technical
University of Sofia.

Title: *Възстановяване на изтрити и повредени видеофайлове при криминалистична
експертиза* (Recovering deleted and damaged video files in forensic examination).

## Scope

- Theory only, in Bulgarian. No program code, no measurements.
- Container and codec are limited to MP4 (ISOBMFF) and H.264.
- Every technical claim cites a standard or a published source. See `REFERENCE_CHECK.md`
  for what was verified and how.
- Length: 13 text pages (Увод to Заключение), 17 PDF pages in all. No length rule from
  the lecturer is recorded yet; 10 to 15 text pages was the working target.

## Contents

| Path | What it is |
|---|---|
| `main.tex` | Skeleton: title page, contents, chapter order, bibliography. |
| `chapters/` | The text. `00` introduction, `01` MP4 and H.264 structure, `02` causes of loss, `03` recovery methods, `04` procedure and evidential value, `05` conclusion. |
| `preamble.tex` | ФКСТ format, copied from `waypoint-communication-networks/docs/preamble.tex` with the Waypoint-only macros removed. |
| `references.bib` | 14 sources. |
| `REFERENCE_CHECK.md` | Status of every reference. |
| `images/tu-logo.png` | Title page logo, from Waypoint. |

## Building

```bash
latexmk -pdf main.tex
```

Output goes to `build/main.pdf`. pdfLaTeX, not XeLaTeX. `latexmkrc` adds the repo root to
`BIBINPUTS`; without it MiKTeX's bibtex runs inside `build/` and silently produces an
empty bibliography.

## Open before handing in

- `\TODO{фак. номер}` on the title page. MCSPC05 is an MCSPC subject, so it would be the
  КСиг number. Whether to print it is Alex's call.
- `\TODO{име на преподавателя}`. Three lecturers share the subject (Проф. Плешкова,
  Доц. Манолова, гл. ас. Нешов). Only the one who set the work goes here.
- The length rule and deadline, once the lecturer states them.

## Notes on the format

- No em or en dashes anywhere in the text. The `ieeetr` style turns every `-` in a
  `pages` field into an en dash, so page ranges are written with the `\pp` macro
  (a plain hyphen) instead.
