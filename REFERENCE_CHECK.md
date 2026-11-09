# Reference check, 9 Nov 2026

What each source is cited for, and how far it was checked. "Index" means the
bibliographic record was confirmed by web search on 9 Nov 2026 but the full text was not
read. "Standard" means the claim is basic structure that the standard defines; the
standard itself was not opened in this session. Nothing marked "not opened" should be
trusted further than that.

| Key | Cited for | Status |
|---|---|---|
| `iso14496_12` | Box header (4 byte size, 4 char type, size 1 and size 0 cases); `ftyp`, `moov`, `mdat`; `stbl` tables `stsz`, `stco`/`co64`, `stsc`, `stss`, `stsd`; movie fragments `moof`; frame timing from `moov` tables | Standard, not opened. Edition year 2022 to confirm. |
| `iso14496_14` | MP4 as a profile of ISOBMFF | Standard, not opened. Edition year 2020 to confirm. |
| `iso14496_15` | Length prefixed NAL units in MP4, no start codes; `avcC` holds SPS, PPS and the length field size | Standard, not opened. Edition year 2022 to confirm. |
| `itu_h264` | NAL header bit layout (1 + 2 + 5 bits); NAL types 1, 5, 6, 7, 8; Annex B start code `00 00 01`; IDR definition | Standard, not opened. Edition year 2021 to confirm. |
| `wiegand2003` | I, P, B frames and inter frame dependency | Not opened. Bibliographic data from memory: IEEE TCSVT 13(7), 560 to 576, 2003. |
| `carrier2005` | Deletion marks entries free and leaves data; quick format leaves the data area; file system fragmentation | Not opened. Book, Addison-Wesley 2005. |
| `richard2005scalpel` | Scalpel as a signature based carver with a configuration file | Not opened. DFRWS 2005. |
| `garfinkel2007` | Carving assumes contiguity; fragmentation on used drives is not rare; fast object validation; bifragment gap carving | Index. Digital Investigation 4S, S2 to S12, 2007 (DFRWS 2007). DTIC hosts a PDF. **No fragmentation percentage is quoted in the text**: secondary sources disagree on the figures. |
| `pal2009` | Definition of file carving; extension past two fragments | Index. IEEE SPM 26(2), 59 to 71, 2009, DOI 10.1109/MSP.2008.931081. |
| `na2014` | Frame based recovery using codec specifications; recovers most non overwritten content, not overwritten segments | Index. IEEE TIP 23(2), 517 to 526, Feb 2014, DOI 10.1109/TIP.2013.2285625. Volume, issue and pages confirmed by search on 9 Nov 2026. |
| `untrunc` | Needs a working reference file from the same device; rebuilds the index of a truncated mp4/mov; success not guaranteed | Repository README summary via web search, 9 Nov 2026. |
| `bell2010` | SSD garbage collection can erase freed blocks without a host command, so deleted data may be gone | Index. JDFSL 5(3), article 1, 2010, Murdoch University. Pages not given in the bib entry. Full text not read. |
| `iso27037` | Guidelines for identification, collection, acquisition, preservation; working copy; chain of custody | Standard, not opened. |
| `nist80086` | Four phases (collection, examination, analysis, reporting); hashing to show integrity | Not opened. NIST SP 800-86, 2006. |

## Not cited

The course lectures (Lecture Audio 3 and 4, the 2025 lecture archive, the Biometric
technologies archive) were not read for this work. Lab 3 (speaker identification) was
read and is about audio, so it is not cited either. If the lecturer expects the course
material to be cited, the video lectures inside `Lectures Ciber SP 07 01 2025.zip` are
the place to look.
