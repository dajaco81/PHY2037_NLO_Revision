# Exam Analysis — PHY2037

Cross-year analysis of all three available past papers (2023, 2024, 2025) and four problem sets. Use this to direct revision time.

---

## Topic Frequency Matrix

Mark allocations are shown where known. A topic in **bold** is structurally certain (appears in every paper examined).

| Topic | 2023 | 2024 | 2025 | PS1 | PS2 | PS3 | PS4 | Verdict |
|-------|------|------|------|-----|-----|-----|-----|---------|
| **1PEF vs 2PEF resolution comparison** | Q1[6] | Q1[2,3] | Q2[3,3] | Q11 | — | — | Q2 | CERTAIN every year |
| **χ estimates from E_at** | Q2[3,3] | Q3[2,1] | Q4[4,3] | — | — | Q6 | — | CERTAIN every year |
| **Pulse parameters (E, P_peak, I_peak)** | Q2[4] | Q3[2,2,2] | Q4[2,2,2] | — | — | Q3a,c | — | CERTAIN every year |
| **Lorentz χ(ω) derivation** | Q3[4] | — | Q3[6] | Q1 | Q1 | — | — | CERTAIN (every paper with Lorentz question) |
| **SHG perturbation theory derivation** | Q3[6] | — | Q3[8] | — | — | Q1 | — | CERTAIN every year |
| **Centrosymmetry: χ⁽²⁾ = 0** | Q3[2,2,1,1] | Q4[4] | Q3[2] | — | — | Q1 | — | CERTAIN every year |
| **Jablonski diagram** | Q4[4] | Q1[4] | Q1[4] | — | — | — | — | CERTAIN every year |
| **IR/Raman selection rules** | Q4[2,2] | Q2[4] | Q1[2,2] | — | Q7 | — | — | CERTAIN every year |
| **Vibrational frequency calculation** | Q4[3] | Q2[3] | Q1[3] | Q8 | Q9 | — | — | CERTAIN every year |
| **Phase matching explanation** | Q3 | Q4[4] | Q2[2,3] | — | — | Q2 | Q4 | CERTAIN every year |
| Rayleigh criterion → NA derivation | Q1[4] | — | Q2[2,2] | Q7 | — | — | — | HIGH |
| Time-bandwidth product derivation | Q2[4] | Q3[3] | — | — | — | Q3d | — | HIGH |
| Confocal microscopy (diagram, sectioning) | Q1[5,2,2] | Q1[4] | — | Q11 | — | — | — | HIGH |
| Rayleigh scattering (depth penetration) | Q1[2] | Q1[4] | Q2[2] | — | — | — | — | HIGH |
| NL wave equation from Maxwell's | — | Q4[6] | — | — | — | Q1 | — | HIGH |
| sinc²(ΔkL/2) derivation | — | Q4[6] | — | — | — | Q2 | — | HIGH |
| Mode locking (KLM or SESAM) | — | Q3[6] | Q4[2,3] | — | — | — | — | HIGH |
| Gouy phase → THG interfaces vs FWM bulk | — | Q2[2] | Q2[2] | — | — | — | Q4 | HIGH |
| Parametric vs non-parametric | — | Q1[4] | — | — | — | Q2 | — | HIGH |
| Hydrogen atom / infinite square well | — | Q2[3,2] | Q1[2,2] | — | — | — | — | HIGH |
| CARS wavelength / pulse bandwidth | — | — | Q4[2,2,2] | — | — | — | — | MEDIUM |
| Stokes wavelength calculation | Q4[2] | — | Q1[2] | — | — | — | — | MEDIUM |
| CW vs pulsed power for E_at | Q2[3,4] | — | — | — | — | Q6 | — | MEDIUM |
| IR wavelength (in microns) | Q4[2] | Q2[3] | Q1[3] | — | — | — | — | HIGH |
| Parabolic potential from linear force | Q3[2] | Q4[3] | Q3[2] | — | — | Q1 | — | CERTAIN (easy 2 marks) |
| E_at calculation (derive 5×10¹¹ V/m) | Q2[2] | Q3[2] | Q4[4] | — | — | — | — | HIGH |
| Intensity required for E_at | Q2[4] | Q3[2] | — | — | — | Q6 | — | HIGH |

---

## Key Patterns

### Structural certainty (every year, every paper)
Every paper has:
1. A question combining **resolution comparison** (1PEF vs 2PEF, sometimes 3PEF)  
2. A question combining **χ estimates** + **pulse parameters** (energy, peak power, intensity)  
3. A question containing the **Lorentz/SHG perturbation derivation**  
4. A question with **Jablonski diagram** + **vibrational spectroscopy** (selection rules + one calculation)

The exam always has exactly 4 questions. Looking at 2023–2025:
- Q1 typically: imaging contrast + confocal/2PEF OR resolution + Jablonski
- Q2 typically: resolution OR χ estimates + pulse parameters
- Q3 typically: Lorentz/perturbation derivations OR NL wave equation
- Q4 typically: Jablonski/vibrational OR phase matching/sinc² OR mode locking/CARS

### The exam formula

The module tests the same **six core competencies** every year, rotating their positions:

| Competency | Derivation | Calculation | Explanation |
|------------|-----------|-------------|-------------|
| Linear optics | χ(ω) from Lorentz | FWHM = 0.61λ/NA | Why confocal fails at depth |
| Nonlinear susceptibility | SHG perturbation, centrosymmetry | χ⁽²⁾, χ⁽³⁾ from E_at | Why χ⁽²⁾=0 for symmetric |
| Wave propagation | NL wave equation, sinc² | Phase mismatch Δk | Phase matching strategies |
| Ultrafast pulses | TBP = 0.441 | E_pulse, P_peak, I_peak | Why CW cannot work |
| Imaging contrast | Jablonski transitions | Resolution 1P vs nP | How 2PEF beats confocal |
| Vibrational spectroscopy | — | ν̃ from k and μ_r | IR vs Raman selection rules |

### New in 2024–2025 (watch for 2026)
These appeared recently and are likely to recur:
- **Infinite square well** for molecule size (2024, 2025) — uses E_n = n²π²ℏ²/8mL²
- **Gouy phase** explanation of FWM-bulk vs THG-interface (2024, 2025)
- **Mode locking** as a substantial question (2024: KLM [6 marks]; 2025: SESAM band diagram [5 marks])
- **CARS/SRS pulse design** — why ps not fs (2025 Q4)

---

## Question Structure Details by Year

### 2023 (4 questions, 25 marks each)

**Q1 — Confocal + Resolution + 2PEF** [3+3+5+2+4+6 = 23 → ~25 marks]
- Confocal scattering depth trade-off [3,3]
- Confocal ray diagram + optical sectioning [5,2]
- Scattering limits confocal depth [2]
- Rayleigh criterion → FWHM = 0.61λ/NA [4]
- 1PEF vs 2PEF resolution (350 nm dye, NA=1.2) [6]

**Q2 — χ estimates + E_at + Pulse power**
- Show E_at ≈ 5×10¹¹ V/m [2]
- Estimate χ⁽²⁾, χ⁽³⁾ [3,3]
- Show I_at = 3×10²⁰ W/m² [4]
- CW laser power for 1 µm spot [3]
- Why pulsed lasers needed [2]
- Pulsed (100 fs, 1 MHz) power for same intensity [4]
- TBP = 0.441 derivation [4]

**Q3 — Lorentz oscillator + SHG perturbation**
- Name three forces in equation of motion [3]
- Parabolic potential from linear restoring force [2]
- Derive r(ω) [4]
- Sketch potentials (asymmetric mar² vs symmetric mbr³) [2,2,1,1]
- Second-order equation of motion from perturbation [4]
- SHG susceptibility χ⁽²⁾(2ω;ω,ω) [6]

**Q4 — Jablonski + IR/Raman**
- Jablonski diagram [4]
- Transitions for fluorescence, SHG, IR, CARS [4]
- Parametric vs non-parametric for each [4]
- Colour from electronic absorption [2]
- IR chemical information [2]
- Raman vs IR selection rules [2]
- C-N wavenumber calculation (k=5×10⁵ g s⁻²) [3]
- IR wavelength in microns [2]
- C-N Stokes wavelength at 514 nm excitation [2]

---

### 2024 (4 questions, 25 marks each)

**Q1 — Fluorescence + Confocal + 2PEF + Resolution**
- Jablonski diagram with fluorescence [4]
- Non-parametric explanation [2]
- Confocal 3D imaging diagram [4]
- 2PEF 3D imaging without pinhole + depth [4]
- 1PEF vs 2PEF resolution (480 nm, NA=1.0) [2,3]
- Resolution at depth in scattering tissue [2]
- Chemical specificity, labelling limitations, NLO alternative [4]

**Q2 — Square well + IR/Raman + CRS**
- Infinite square well: L for 500 nm absorption [3]
- Molecular feature example [2]
- Absorption vs 2PA for 3D imaging [5]
- Why IR transitions give more chemical information [4]
- C-H IR wavelength (k=5×10² kg s⁻¹ = 500 N/m) [3]
- IR imaging limitations; how Raman overcomes [4]
- How CRS (CARS/SRS) overcomes weak Raman [4]

**Q3 — Pulse parameters + TBP + KLM**
- χ⁽²⁾ from E_at [2,1]
- χ⁽³⁾ [2,1]
- Intensity for E_at [2]
- Why CW not feasible [2]
- Ti:Saph (120 fs, 900 nm, 40 MHz, 10 mW, 1 µm spot): energy, peak power, peak intensity [2,2,2]
- TBP: bandwidth in nm [3]
- KLM description [6]

**Q4 — Centrosymmetric oscillator + NL wave equation + sinc²**
- Significance of mbx³ term; sketch potential [3]
- Symmetric potential → χ⁽²⁾ = 0 (power series) [4]
- Nonlinear wave equation from Maxwell's [6]
- Role of P_NL [2]
- Sinc² derivation from dA₃/dz equation [6]
- Sketch I₃ vs ΔkL; significance of ΔkL = π [4]

---

### 2025 (4 questions, 25 marks each)

**Q1 — Hydrogen atom + Square well + Jablonski + IR/Raman**
- Hydrogen atom levels → UV only, no visible contrast [2]
- Square well: molecule size for 500 nm absorption [2]
- Electronic vs vibrational contrast (chemical specificity) [2,2]
- Jablonski → fluorescence [4]
- Jablonski for IR absorption and Raman scattering [1,1]
- N-H IR wavelength + Raman Stokes at 785 nm [3,2]
- IR imaging limitations; how Raman overcomes [3,3]

**Q2 — Resolution + Rayleigh scattering + Phase matching + Gouy phase**
- Resolution at 532 nm and 1064 nm (NA=1.2) [2,2]
- Rayleigh scattering ratio (532 vs 1064 nm) [2]
- Scattering limits confocal depth [2]
- NLO extends depth without resolution loss [4]
- 2nd and 3rd order NLO resolution at 1064 nm (NA=1.2) [3,3]
- Phase matching importance for parametric processes [2]
- Normal dispersion prevents phase matching (SFG example) [3]
- Gouy phase: FWM bulk vs THG interfaces [2]

**Q3 — Lorentz oscillator + SHG perturbation**
- Parabolic potential [2]
- χ_e(ω) derivation [6]
- Sketch amplitude and phase vs frequency [5]
- Asymmetric potential sketch [2]
- SHG χ⁽²⁾ derivation from perturbation [8]
- Why χ⁽²⁾ = 0 for symmetric [2]

**Q4 — χ⁽³⁾ + Ultrafast necessity + CARS pulse params + SESAM**
- Calculate E_at (more precisely: 5.14×10¹¹ V/m); χ⁽³⁾ = 3.78×10⁻²⁴ m²/V² [4,3]
- Why ultrafast excitation essential [5]
- CARS laser (1 ps, 1064 nm, 80 MHz, 10 mW): energy, peak power, bandwidth [2,2,2]
- Why shorter pulses NOT beneficial for CARS [2]
- Saturable absorber band diagrams [2,3]

---

## Gaps in Current Revision Materials

The following topics appear in real papers but are **not fully covered** in the existing `05_exam_prep/` files. They have been addressed in `PAST_PAPER_SOLUTIONS.md` and new model questions Q13–Q20 have been added to `05_exam_prep/MODEL_QUESTIONS.md`.

| Gap | Where addressed | Mark value |
|-----|----------------|-----------|
| Infinite square well → molecule size | MODEL_QUESTIONS Q13 | 2–3 marks |
| Hydrogen atom → UV only | MODEL_QUESTIONS Q14 | 2 marks |
| CW vs pulsed power comparison | MODEL_QUESTIONS Q15 | 3+4 marks |
| Stokes wavelength + IR wavelength calculation | MODEL_QUESTIONS Q16 | 2+2 marks |
| KLM mode locking [6 mark description] | MODEL_QUESTIONS Q17 | 6 marks |
| Gouy phase: FWM bulk vs THG interface (phase argument) | MODEL_QUESTIONS Q18 | 2 marks |
| CARS pulse parameters + bandwidth (in nm) | MODEL_QUESTIONS Q19 | 2+2+2 marks |
| Rayleigh scattering ratio calculation | MODEL_QUESTIONS Q20 | 2 marks |
| Raman Taylor expansion (induced polarization) | PROBLEM_SET_SOLUTIONS | 7 marks |
| Plasma frequency explanation | PROBLEM_SET_SOLUTIONS | 2 marks |
| Normal vs anomalous dispersion | PROBLEM_SET_SOLUTIONS | 3 marks |

---

## Mark-per-Minute Strategy

2 hours for 100 marks = **1.2 minutes per mark**.

| Mark type | Time budget | Strategy |
|-----------|------------|----------|
| [2] marks (parabolic potential, E_at, selection rules) | ~2.5 min | Never skip — easy marks, formulaic |
| [4] mark calculations (FWHM, TBP, Jablonski) | ~5 min | Must be fast and correct |
| [6] mark derivations (χ(ω), sinc², NL wave eq.) | ~7 min | Know the 4-5 steps cold |
| [8] marks (SHG perturbation, 2025 Q3) | ~10 min | Biggest single question — know every step |

The [2]-mark "parabolic potential" question **appears in every paper** (2023 Q3, 2024 Q4, 2025 Q3). It is 2 guaranteed marks for writing: V = ½mω₀²r² (integration of restoring force F = −mω₀²r).
