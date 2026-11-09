# Reference check, 9 Nov 2026

Every source was looked up again on 9 Nov 2026, this time in the primary text where it
could be reached. Each row says what was actually read.

## Read in full

| Key | Cited for | Verdict and location |
|---|---|---|
| `itu_h264` | NAL header 1 + 2 + 5 bits, `forbidden_zero_bit` = 0; types 1, 5, 6, 7, 8; Annex B start code `0x000001`; IDR; PPS refers to SPS; SPS holds profile and frame size | Confirmed in the 08/2021 and 06/2026 editions (itu.int PDFs). Clauses 7.3.1, 7.4.1, Table 7-1, 3.69 (IDR), Annex B.1, 7.4.2.2, 7.3.2.1.1. The two editions agree on all of these. Cited as 2026, the edition in force. |
| `wiegand2003` | I, P, B frames; inter prediction from decoded pictures; NAL units; IDR | Confirmed, pp. 562, 564, 566. TCSVT 13(7):560 to 576, July 2003. |
| `nist80086` | Deleted file: pointer marked deleted, data stays until overwritten (§4.1.3); four phases (§3); work only on the copy (p. 3-4, §4.2); message digests to verify integrity (p. 3-4, 4-8); chain of custody | Confirmed. August 2006. Now also carries the deletion claim and the chain of custody claim. |
| `garfinkel2007` | Carvers assume contiguity; fragmentation statistics; fast object validation; bifragment gap carving | Confirmed (Introduction S3, §3.2 Table 1, §4.1, §5.2.1). **Corrected:** the text said fragmentation is "not rare". Garfinkel reports about 6% of files fragmented over 300+ drives, half the drives with none, 30 drives above 10%, and calls it "relatively rare" while still treating fragment carving as necessary. The text now says exactly that. |
| `richard2005scalpel` | Header/footer carver driven by a configuration file, efficient scanning | Confirmed, §2.1.2. DFRWS 2005, pp. 71 to 77. Conference city not confirmed, so it was removed. |
| `bell2010` | SSD garbage collection erases freed data without a host command; quick-formatted HDD kept all data; quick-formatted SSD wiped itself in about three minutes | Confirmed, abstract and pp. 7 to 10. JDFSL 5(3):1 to 20, 2010. |

## Abstract or record only

| Key | Cited for | Verdict |
|---|---|---|
| `na2014` | Frame-based recovery using codec specifications; most content in non-overwritten segments recovered | Confirmed from the verbatim abstract (Europe PMC). IEEE TIP 23(2):517 to 526, 2014. Full text paywalled. |
| `pal2009` | Carving as recovery without file system metadata; history of carving | Confirmed from the abstract. **Removed:** the claim that the paper covers more than two fragments, which the abstract does not show. |
| `untrunc` | Needs a working file from the same camera or app; restores truncated mp4/mov; "some luck" needed | Confirmed from the README. **Corrected:** the README does not describe how it works, so the text no longer says what untrunc does internally. It now explains, from the format alone, why a reference file is needed. |

## Not readable without an ISO account or purchase

| Key | Cited for | Status |
|---|---|---|
| `iso14496_12` | Box header, size 1 and size 0; `ftyp`, `moov`, `mdat`; `stbl` tables; `moof`; timing from `moov` | **Not verified against the standard.** ISO's free-standards page is closed; ISO/IEC 14496-12:2026 (edition 8, the one in force) is listed at CHF 0 but needs an ISO account to download. 2022 edition withdrawn. The `ftyp` wording was softened to "as early as possible" and the byte 4 to 7 signature made conditional on `ftyp` being first. |
| `iso14496_14` | MP4 is a specialisation of ISOBMFF | Not verified. 2020 edition confirmed in force from the ISO catalogue. |
| `iso14496_15` | Length-prefixed NAL units; `avcC` holds SPS, PPS, length size | Not verified. 2024 edition in force; 2022 withdrawn. |
| `iso27037` | Scope: identification, collection, acquisition, preservation | Only the title and scope confirmed from the ISO catalogue. The working copy and chain of custody claims are now cited to NIST SP 800-86 instead. |

## Removed

- `carrier2005` (*File System Forensic Analysis*). No legal preview could be read. Its
  claims are now cited to NIST SP 800-86, Bell and Boddington, and Garfinkel, which were
  read.

## Course material

Not cited. The lectures were not read; Lab 3 is about audio.
