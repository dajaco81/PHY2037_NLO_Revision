# PHY2037 Master Revision Map

This document provides a complete topic-by-topic roadmap of the module. Use this as your primary orientation document.

---

## Module Arc

The module builds from fundamental physics to cutting-edge imaging technology in nine topics:

```
ATOMS                                          IMAGES
  │                                               │
  ▼ light–matter                                  │
  P = ε₀χE                                        │
  │ polarisation                                   │
  ▼ linear                                         │
  Lorentz oscillator → χ(ω)                        │
  │                                               │
  ▼ nonlinear                                      │
  Power series → χ₂, χ₃                            │
  │                                               │
  ▼ wave optics                                    │
  NL wave equation → phase matching               │
  │                                               │
  ▼ practical                                      │
  Ultrafast lasers + NLO microscopy               │
  │                                               │
  └────────────────────────────────────────────►──┘
```

---

## Topic 1: Introduction (L01–L02)

**What:** Course overview + prerequisite physics recap.

**Key physics:**
- The central equation: **P = ε₀χE** — susceptibility χ contains all material information
- Power series: **P = ε₀[χ⁽¹⁾E + χ⁽²⁾E² + χ⁽³⁾E³ + …]**
- Intensity: I = ½cε₀E²
- Harmonic oscillator resonance (swing analogy)
- Atomic field strength: E_at ≈ 5×10¹¹ V/m
- FWHM of Gaussian: FWHM = 2√(2ln2)·σ
- Fourier transform: FT of Gaussian is a Gaussian; shorter pulse ↔ wider bandwidth
- **Critical conversion:** Δλ = (λ²/c)·Δν (NOT linear)

**Why it matters:** The power series is the foundation of all NLO. The FWHM and FT relations return repeatedly (resolution, pulse characterisation). E_at is used to estimate χ₂ and χ₃.

---

## Topic 2: Optical Imaging (L03–L04)

**What:** How we form images with light — contrast, resolution, 3D imaging, and the scattering problem.

**Key physics:**
- **Contrast mechanisms:** absorption (Beer-Lambert: A = εcl), fluorescence (Stokes shift, Jablonski diagram), Rayleigh scattering (I ∝ 1/λ⁴)
- **Molecular colour:** conjugated π-bonds, L ≈ 0.67 nm for visible absorption
- **Labelling limitations:** tag must be small relative to molecule ("elephant and GPS tag")
- **Numerical aperture:** NA = n·sinα
- **Abbe diffraction limit:** d = λ/(2·NA); derived from angular Rayleigh criterion
- **Confocal microscopy:** pinholes at excitation and detection reject out-of-plane light → optical sectioning
- **The tradeoff:** resolution ∝ λ vs. scattering ∝ λ⁻⁴ vs. contrast mechanism dictates λ → cannot simultaneously optimise with linear optics

**Why it matters:** This is the problem NLO solves. Every advantage of 2PEF/SHG/CARS traces back to overcoming one of the limitations introduced here.

---

## Topic 3: Linear Light–Matter Interaction (L05–L07)

**What:** How to derive χ(ω) and understand vibrational spectroscopy.

**Key physics:**
- **Lorentz oscillator:** mṙ̈ + mγṙ + mω₀²r = qE₀e^{-iωt}; solution gives χ⁽¹⁾(ω) = Nq²/(mε₀) / [(ω₀²−ω²) − iγω]
- **Polarisation timescales:** electronic (fs, UV-vis) → atomic/vibrational (ps, IR) → orientational (µs, microwave)
- **Chemical specificity:** only atomic polarisation gives molecular fingerprint
- **IR selection rule:** change in dipole moment (dμ/dQ ≠ 0)
- **Raman selection rule:** change in polarizability (dα/dQ ≠ 0)
- **Vibrational frequency:** ν = (1/2π)√(k/μ_r), μ_r = m₁m₂/(m₁+m₂)
- **Wavenumber unit:** $\tilde{\nu}$ = 1/λ in cm⁻¹
- **Raman sideband derivation:** cos A·cos B → frequency sidebands at ω_L ± ω_vib

**Why it matters:** The Lorentz oscillator derivation is the blueprint for the nonlinear extension. IR and Raman are the linear baselines that CARS/SRS improve upon.

---

## Topic 4: Nonlinear Susceptibilities (L08–L09)

**What:** The power series in detail — estimates, symmetry, and derivation of χ⁽²⁾.

**Key physics:**
- **χ estimates:** χ⁽²⁾ ≈ 2×10⁻¹² m/V; χ⁽³⁾ ≈ 4×10⁻²⁴ m²/V² (tiny → need extreme intensities)
- **Units:** χ⁽¹⁾ dimensionless; χ⁽²⁾ in m/V; χ⁽³⁾ in m²/V²
- **Centrosymmetry:** χ⁽²⁾ = 0 for centrosymmetric materials (symmetric restoring force)
- **Perturbation technique:** r = λr₁ + λ²r₂ + …; collect terms at each order of λ
- **SHG derivation:** second-order EOM driven by r₁² → gives χ⁽²⁾(2ω;ω,ω)
- **SFG, DFG:** same method, different target frequency

**Why it matters:** χ⁽²⁾ derivation is likely an exam question. The centrosymmetry argument explains why SHG only works for special materials (collagen, BBO, quartz).

---

## Topic 5: Wave Equation and Phase Matching (L10–L11)

**What:** How NLO signals propagate and how to make them efficient.

**Key physics:**
- **Nonlinear wave equation:** ∇²E − (n²/c²)∂²E/∂t² = (1/ε₀c²)∂²P_NL/∂t²
- **Phase matching:** k₁ + k₂ = k₃ (Δk = 0); signal grows as L → intensity ∝ N²
- **sinc² profile:** I₃ ∝ L² sinc²(ΔkL/2); first zero at ΔkL/2 = π
- **Coupled amplitude equations:** dA₃/dz = (iω₃d_eff/n₃c)A₁A₂e^{iΔkz}; derived via SVEA
- **Normal dispersion prevents perfect PM:** n(2ω) > n(ω) always → Δk ≠ 0
- **Phase matching schemes:** angle tuning, temperature tuning (LiNbO₃), quasi-PM (PPLN, period = π/Δk)
- **Gouy phase shift:** π total through focus; SHG: L < λ/2; THG: L < λ/3

**Why it matters:** Phase matching is why NLO processes are weak without engineering; the sinc² formula is used in applications (EPI-CARS). Both wave equation and coupled amplitude equation derivations are examinable.

---

## Topic 6: Laser Pulses (L12, L14)

**What:** Why we use ultrashort pulses and how to characterise them.

**Key physics:**
- **Required intensity:** ~3×10²⁰ W/m² → only achievable by temporal squeezing
- **Pulse parameters:** E_pulse = P_av/f_rep; P_peak = E_pulse/τ; I_peak = P_peak/A
- **Bandwidth:** Δν·Δt = 0.441 (time-bandwidth product, Gaussian pulses); Δλ = (λ²/c)Δν
- **Chirped pulses:** GVD stretches pulses in dispersive media (red arrives first in normal dispersion)
- **Pulse formation:** superposition of many wavelengths locked in phase

**Why it matters:** All NLO signal calculations require these. TBP derivation is a likely exam question. Bandwidth conversion is tested every year.

---

## Topic 7: Nonlinear Optical Microscopy (L14–L16)

**What:** How NLO overcomes the limitations of conventional microscopy.

### Key advantages of NLO microscopy:
1. **No pinhole** — signal only from focal spot (intrinsic confinement)
2. **Deeper penetration** — 2× excitation wavelength → 16× less scattering
3. **Resolution partially recovered** — nonlinear squeeze: d_nP = d_1P/√n (for same target molecule)

### 2PEF (Two-Photon Excited Fluorescence)
- Two IR photons → excite same fluorescent dye as one UV/visible photon
- Scales as I² → intrinsically confocal
- Depth: ~800 µm in brain vs. ~100 µm for 1PEF
- Parametric? No (fluorescence = non-parametric)

### SHG (Second Harmonic Generation)
- Second-order process (χ⁽²⁾); 2ω₁ → ω₂ = 2ω₁
- Parametric; phase matching needed (L < λ/2 in tight focus via Gouy)
- Only non-centrosymmetric structures: **collagen** and **myosin**
- Label-free intrinsic contrast

### THG (Third Harmonic Generation)
- Third-order; 3ω₁ → ω₂ = 3ω₁
- Phase matching condition: L < λ/3 → only interfaces and sub-λ objects
- Interface-selective contrast

### CARS (Coherent Anti-Stokes Raman Scattering)
- Four-wave mixing: 2ω_P − ω_S = ω_AS; tune ω_P − ω_S = ω_vib
- Coherent driving → enhanced Raman; video-rate imaging possible
- Problem: non-resonant electronic background in every pixel
- Wavelength calculation: λ_S = 1/(1/λ_P − ν̃_vib); λ_AS = 1/(1/λ_P + ν̃_vib)
- Need picosecond pulses to resolve individual Raman peaks

### SRS (Stimulated Raman Scattering)
- Non-parametric; no electronic background → cleaner images than CARS
- Detected via modulation transfer with lock-in amplifier
- Signal: pump depletion at ω_P (SRL) or Stokes gain at ω_S (SRG)

---

## Topic 8: Laser Sources (L17)

**What:** How ultrafast lasers are built and how to generate multiple synchronized wavelengths.

- **Mode locking:** SESAM (ps pulses, semiconductor absorber) or KLM (fs pulses, Kerr lens)
- **Dispersion compensation:** grating or prism pairs inside cavity
- **Ti:Sapphire:** typical NLO laser (690–1080 nm, ~80 MHz, ~100 fs, ~700 mW)
- **Synchronisation:** electronic (Keltner, ~20 fs jitter) or optical injection locking (< 5 fs jitter)
- **Frequency conversion:** SHG (λ/2) and OPO (1/λ_P = 1/λ_S + 1/λ_i) for tunable second wavelength

---

## Topic 9: Applications (L18)

**What:** Real-world impact of NLO microscopy.

- **EPI-CARS / backward phase matching:** sub-wavelength particle detection (nanoparticle drug delivery, microplastics)
- **Virtual H&E + AI:** label-free cancer diagnosis from SRS images
- **Deuterium labelling:** D replaces H → C–D stretch at ~2100 cm⁻¹ (silent region); minimal chemical perturbation
- **Drug skin penetration:** SRS imaging of drug + solvent diffusion
- **SHG applications:** collagen in arthritis/fibrosis; myosin in muscular dystrophy

---

## Critical Connections

| NLO advantage | Problem solved (from Topic 2) |
|---------------|------------------------------|
| No pinhole | Scattering defeats confocal detection |
| 2× wavelength excitation | Scattering I ∝ λ⁻⁴ — longer λ penetrates deeper |
| Decouples excitation from emission λ | Contrast mechanism dictates λ |
| SHG/CARS for label-free | Labelling perturbs small molecules |
| 1/√n resolution recovery | "Wasted" factor of n in excitation wavelength |
| EPI-CARS nanoparticles | Phase matching makes sub-λ selective |
