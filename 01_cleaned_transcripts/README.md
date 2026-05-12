# 01_cleaned_transcripts — Cleaned Lecture Transcripts

Cleaned versions of the raw transcripts. Pre-lecture chatter, repetitive filler, and transcription noise have been removed. All physics content, equations, examples, exam hints, and lecturer comments are preserved.

## Cleaning Rules Applied

- Pre-lecture chatter and post-lecture conversations removed
- Repeated filler phrases and obvious transcription errors removed
- Physics content preserved verbatim (including uncertain/garbled technical statements, flagged with `[UNCLEAR]`)
- Equations not silently corrected — any correction is noted with `[INFERRED CORRECTION: ...]`
- Lecturer exam hints preserved and tagged: `[EXAM HINT]`, `[RED BOX]`, `[COMMON MISTAKE]`

## File Naming

`L{number}_{YYYY-MM-DD}_cleaned.md`

Each file includes YAML frontmatter with lecture metadata and confidence rating.

## Confidence Levels

- **high**: Transcript is coherent, physics content is clear
- **medium**: Some noise but main physics is recoverable  
- **low**: Heavily corrupted, incomplete, or mostly non-physics content
