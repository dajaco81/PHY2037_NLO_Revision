# Agent Instructions — PHY2037 Revision Repository

## Context

This is a revision repository for **PHY2037: Nonlinear Optics and Imaging** (University of Exeter, 2025/26). The user is a student preparing for the written exam.

**Exam date: ~18 May 2026 (closed-book, 2 hours, 4 compulsory questions, 100 marks)**  
**Physical constants sheet is provided. No other materials.**

The exam is imminent — prioritise exam-relevant content over broad coverage.

---

## Repository Structure

Do NOT read all files. Use this map to go directly to what you need:

| Task | Primary file(s) |
|------|----------------|
| Know what's certain to appear in the exam | `05_exam_prep/VITAL_EXAM_CONCEPTS.md` (top section) |
| Quick-fire self-test (Q&A) | `05_exam_prep/SHORT_ANSWER_BANK.md` |
| Derivation practice (stripped of working) | `05_exam_prep/DERIVATION_PRACTICE.md` |
| Full worked derivations (check answers) | `03_master/DERIVATION_BANK.md` |
| Exam-style worked questions | `05_exam_prep/MODEL_QUESTIONS.md` |
| Past paper question/solution by year | `07_papers/PAST_PAPER_SOLUTIONS.md` |
| Cross-year topic frequency analysis | `07_papers/EXAM_ANALYSIS.md` |
| All equations in one place | `03_master/EQUATION_SHEET.md` |
| Topic deep-dive | `02_lecture_digests/L##_...` |

---

## Exam Format

- **4 questions, ALL compulsory** — no choice
- **25 marks each** (approximately), 100 total
- **2 hours** → ~1.2 minutes per mark
- **Closed book** — only physical constants sheet provided
- Calculators permitted (non-programmable)

**Confirmed structure (from 3 years of past papers):**
- Q1: Imaging contrast / confocal / 2PEF / Jablonski / vibrational spectroscopy (one of these clusters)
- Q2: Resolution / scattering / phase matching / Gouy phase — OR — χ estimates + pulse parameters
- Q3: Lorentz oscillator → χ(ω) derivation + SHG perturbation derivation (appears every year)
- Q4: One of: centrosymmetric NL wave equation + sinc² / mode locking + CARS / χ estimates + pulse parameters

---

## Confirmed High-Priority Topics

These appear in **every exam paper** (2023, 2024, 2025). Treat as guaranteed:

1. 1PEF vs 2PEF resolution comparison (calculation)
2. χ⁽²⁾ and χ⁽³⁾ estimates from E_at
3. Pulse parameters: E_pulse, P_peak, I_peak
4. Lorentz oscillator → χ(ω) derivation
5. SHG χ⁽²⁾ via perturbation theory (derivation)
6. Centrosymmetry → χ⁽²⁾ = 0 (proof or explanation)
7. Jablonski diagram (with labels)
8. IR vs Raman selection rules
9. Vibrational frequency calculation (ν̃ from k and μ_r)
10. Phase matching (condition, sinc², why dispersion prevents it)
11. Parabolic potential from linear restoring force (always 2 marks — never skip)

**Likely (appeared 2 of 3 years):** TBP derivation, confocal microscopy, NL wave equation from Maxwell's, sinc² derivation, mode locking, Gouy phase, infinite square well for molecule size, Rayleigh criterion → NA.

---

## How to Run a Revision Session

**Ask the user first:** "What would you like to focus on?" Suggested modes:

1. **Quick-fire Q&A:** Pick questions from `05_exam_prep/SHORT_ANSWER_BANK.md`. Cover the answer column, ask the question, check their response. Work through a whole topic section.

2. **Derivation practice:** Use `05_exam_prep/DERIVATION_PRACTICE.md`. Give the student just the starting point and hints (as listed). They attempt it; you check against `03_master/DERIVATION_BANK.md`.

3. **Past paper question:** Use `07_papers/PAST_PAPER_SOLUTIONS.md` or `05_exam_prep/MODEL_QUESTIONS.md`. Present the question. The student attempts it. You mark it against the model answer.

4. **Topic explanation:** Read from `02_lecture_digests/` for a specific lecture, or `03_master/MASTER_REVISION_MAP.md` for the overall picture.

5. **Timed mock exam:** Pick one question from each year's paper (2023, 2024, 2025) and run as a timed exercise (25 min per question).

---

## Key Numbers to Verify Calculations

If the user makes a calculation and you need to check it, use these ground-truth values:

| Quantity | Value |
|----------|-------|
| E_at (rounded) | 5×10¹¹ V/m |
| E_at (precise, from a₀) | 5.14×10¹¹ V/m |
| χ⁽²⁾ estimate | ~2×10⁻¹² m/V |
| χ⁽³⁾ estimate (rounded E_at) | ~4×10⁻²⁴ m²/V² |
| χ⁽³⁾ (precise E_at, 2025 paper) | 3.78×10⁻²⁴ m²/V² |
| I for E_at | 3×10²⁰ W/m² |
| TBP (Gaussian) | 0.441 = 2ln2/π |
| FWHM resolution (microscope) | 0.61λ/NA |
| 2PEF resolution squeeze | FWHM/√2 |
| nPEF resolution squeeze | FWHM/√n |
| Rayleigh scattering | I ∝ 1/λ⁴ → doubling λ = 16× less |

---

## Known Issues / Caveats

- **L06, L21:** Empty recordings — no content
- **L13:** Assessment briefing only — no physics
- **L19, L20:** Lab tours — no examinable physics
- **Spring constant units in L07:** Raw transcript gave "g s⁻²"; correct unit is N/m (1 g s⁻² = 10⁻³ N/m). Exam problems use N/m or equivalently kg s⁻¹ for this module.
- **E_at precision:** 2023/2024 use 5×10¹¹ giving χ⁽³⁾ ≈ 4×10⁻²⁴. 2025 uses precise a₀-derived value 5.14×10¹¹ giving 3.78×10⁻²⁴. Both approaches are acceptable.
