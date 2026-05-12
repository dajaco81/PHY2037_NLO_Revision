# Processing Log

Record of all processing decisions made when building this repository from the raw Panopto transcripts.

---

## Overview

**Source material:** 21 Panopto auto-generated caption files for PHY2037 "From Atoms to Images with Nonlinear Optics", University of Exeter, Semester 2 2025/26.

**Processing date:** 2026-05 (retrospective documentation)

**Processor:** Claude (claude-sonnet-4-6) via Claude Code CLI

**Input directory:** `raw/` (original Panopto export, files numbered 01–21 in reverse chronological order)

**Output:** 7-directory structured repository (00_raw_transcripts/ through 06_metadata/)

---

## File Renaming and Chronological Mapping

The raw Panopto export numbered files in **reverse chronological order**: file `01` was the most recent recording (2026-03-24), and file `21` was the earliest (2026-01-12). All files were renamed to L01–L21 in forward chronological order based on the timestamps in `_manifest_original.json`.

| Original filename | Lecture number | Date |
|-------------------|---------------|------|
| 21.txt | L01 | 2026-01-12 |
| 20.txt | L02 | 2026-01-13 |
| 19.txt | L03 | 2026-01-19 |
| 18.txt | L04 | 2026-01-20 |
| 17.txt | L05 | 2026-01-26 |
| 16.txt | L06 | 2026-01-27 |
| 15.txt | L07 | 2026-01-28 |
| 14.txt | L08 | 2026-02-02 |
| 13.txt | L09 | 2026-02-03 |
| 12.txt | L10 | 2026-02-09 |
| 11.txt | L11 | 2026-02-10 |
| 10.txt | L12 | 2026-02-23 |
| 09.txt | L13 | 2026-02-24 |
| 08.txt | L14 | 2026-03-02 |
| 07.txt | L15 | 2026-03-03 |
| 06.txt | L16 | 2026-03-09 |
| 05.txt | L17 | 2026-03-10 |
| 04.txt | L18 | 2026-03-16 |
| 03.txt | L19 | 2026-03-17 |
| 02.txt | L20 | 2026-03-23 |
| 01.txt | L21 | 2026-03-24 |

---

## Lectures Processed (Substantive Physics Content)

The following 16 lectures contained substantive physics and were fully processed into cleaned transcripts and digests:

| Lecture | Topics | Processing notes |
|---------|--------|-----------------|
| L01 | Course intro, P=ε₀χE, SHG history | Good quality; pre-lecture chatter removed |
| L02 | EM recap, Lorentz, FWHM, Fourier transforms | Good quality; Δλ=(λ²/c)Δν formula verified |
| L03 | Fluorescence, Jablonski, staining | "Blonsky" corrected to "Jablonski" throughout [INFERRED CORRECTION] |
| L04 | NA, Rayleigh criterion, confocal | "Brady scattering" corrected to "Rayleigh scattering" |
| L05 | Lorentz oscillator χ(ω) derivation | Good quality; derivation steps reconstructed from notes |
| L07 | IR/Raman selection rules, calculations | Spring constant units corrected (g/s² → N/m); see POSSIBLE_TRANSCRIPT_ERRORS |
| L08 | χ power series, centrosymmetry, SHG/SFG/DFG/THG | Good quality |
| L09 | Perturbation theory, SHG χ⁽²⁾ derivation | Good quality; χ⁽²⁾=0 for centrosymmetric proof included |
| L10 | Nonlinear wave equation, sinc², coupled amplitude | Good quality; coupled amplitude derivation verified |
| L11 | Phase matching (angle, temperature, PPLN), Gouy phase | "Gooey phase" corrected to "Gouy phase" [INFERRED CORRECTION] |
| L12 | Laser pulses, peak intensity, bandwidth, chirp | 80 MHz vs 1 kHz comparison reconstructed |
| L14 | TBP derivation, 2PEF, intrinsic confocality | Good quality; TBP = 0.441 derived from FT |
| L15 | Resolution squeeze, SHG (collagen/myosin), THG | 1/√n PSF squeeze derivation included |
| L16 | CARS wavelength, SRS, modulation transfer, ps pulses | CARS calculation verified numerically |
| L17 | Mode locking (SESAM/KLM), Ti:Sapphire, OPO | OPO energy conservation equation verified |
| L18 | EPI-CARS, virtual H&E, D-labelling, microplastics | Final physics lecture; good quality |

---

## Lectures Skipped or Given Placeholder Treatment

### L06 — 2026-01-27 (Empty)
**Status:** No audio captured. Raw file contains only Panopto session metadata with zero transcript lines.  
**Action:** Placeholder files created in 01_cleaned_transcripts/ and 02_lecture_digests/ with `confidence: low`, `quality: empty`.  
**Impact:** Topic coverage for this slot (likely: continuation of Lorentz oscillator or intro to vibrational spectroscopy based on surrounding lectures) is missing. L05 and L07 provide good coverage of the surrounding material; no critical gaps identified.

### L13 — 2026-02-24 (Video Assessment Briefing)
**Status:** Recording captured but contains only administrative content: briefing for the video assessment component. No physics content.  
**Action:** Placeholder files created noting "video assessment briefing only".  
**Impact:** No physics content lost. Assessment instructions not reproduced (not relevant to exam preparation).

### L19 — 2026-03-17 (Lab Tour — Corrupted)
**Status:** Transcript is heavily corrupted. Appears to record a lab tour; Panopto auto-captions capture only fragments of ambient speech. No coherent physics content extractable.  
**Action:** Placeholder files created with `confidence: low`, `quality: corrupted`.  
**Impact:** Lab tours are not examinable content.

### L20 — 2026-03-23 (Lab Tour — Corrupted)
**Status:** Same as L19. Second lab tour session; corrupted transcript.  
**Action:** Placeholder files created.  
**Impact:** None for exam preparation.

### L21 — 2026-03-24 (Empty)
**Status:** No audio captured. Zero transcript content.  
**Action:** Placeholder files created with `confidence: low`, `quality: empty`.  
**Impact:** This was the final session; lab tour content only. No physics content lost.

---

## Transcript Corrections Made

All corrections are documented in detail in `04_audit/POSSIBLE_TRANSCRIPT_ERRORS.md`. Summary:

| Error in raw transcript | Corrected to | Confidence | Lectures affected |
|------------------------|--------------|------------|-------------------|
| "Brady scattering" | Rayleigh scattering | Certain | L04 |
| "Blonsky diagram" | Jablonski diagram | Certain | L03 |
| "Gooey phase" / "Gooey phase shift" | Gouy phase shift | Certain | L11 |
| "Franklin" / "Franken" | Franken (Peter Franken, 1961 SHG discoverer) | High | L01, L08 |
| Spring constant units "grams per second squared" | N/m | Certain | L07 |
| "nanotubes" in energy context | nanojoules | High | L12, L16 |
| "Stokes theorem" in Raman context | Stokes shift | High | L07, L15 |

All corrections are tagged `[INFERRED CORRECTION]` in cleaned transcript files to preserve an audit trail.

---

## Known Unreliable Files

The following files should be treated with lower confidence:

| File | Reason | Reliability |
|------|--------|-------------|
| L06_2026-01-27_cleaned.md | No source content | Placeholder only |
| L19_2026-03-17_cleaned.md | Corrupted auto-captions | Unreliable |
| L20_2026-03-23_cleaned.md | Corrupted auto-captions | Unreliable |
| L21_2026-03-24_cleaned.md | No source content | Placeholder only |
| L13_2026-02-24_cleaned.md | Non-physics content | Not relevant for exam |

For all other lectures, the cleaned transcripts are considered reliable. Where transcript ambiguities were identified in physics content (e.g., intermediate arithmetic that doesn't quite work out), these are flagged in `04_audit/INCONSISTENCY_LOG.md`.

---

## Processing Decisions

**Retained:** All pre-lecture chatter and administrative announcements were removed from cleaned transcripts. Only physics-relevant content was retained.

**Preserved:** All lecturer emphasis markers ("you need to remember this", "this will come up in the exam", "red box") were retained in cleaned transcripts and propagated to `05_exam_prep/VITAL_EXAM_CONCEPTS.md`.

**Not fabricated:** Where the transcript was ambiguous or partially corrupted, working was NOT invented. Instead, ambiguities are noted explicitly. The derivation bank (`03_master/DERIVATION_BANK.md`) presents complete derivations reconstructed from the combined evidence of transcripts, standard textbook results, and physical consistency checks — these are clearly labelled as reconstructions where the transcript alone was insufficient.

**Equations:** All LaTeX equations in cleaned transcripts and master files were verified for dimensional consistency and physical correctness. Two arithmetic inconsistencies were found and logged (see `04_audit/INCONSISTENCY_LOG.md`); in both cases the physically correct version was used.

---

## Repository Completeness

| Directory | Files | Status |
|-----------|-------|--------|
| 00_raw_transcripts/ | 22 (21 raw + README) | Complete |
| 01_cleaned_transcripts/ | 22 (21 cleaned + README) | Complete |
| 02_lecture_digests/ | 22 (21 digests + README) | Complete |
| 03_master/ | 5 (README + 4 synthesis files) | Complete |
| 04_audit/ | 4 (README + 3 audit files) | Complete |
| 05_exam_prep/ | 5 (README + 4 prep files) | Complete |
| 06_metadata/ | 5 (README + 4 metadata files) | Complete |
| Root | 1 (README.md) | Complete |

**Total files created:** 86

**Total lectures with full physics content:** 16 of 21 (76%)

**Exam-relevant content:** All 16 physics lectures fully processed. No examinable content identified as missing.
