# Short Answer Bank

Quick-fire Q&A for self-testing. Cover the right column and test yourself.

---

## Fundamentals

| Question | Answer |
|----------|--------|
| What does χ (electric susceptibility) physically represent? | How easily a material's bound charges can be polarised by an applied electric field; it is frequency-dependent and contains all information about the material's optical response |
| What are the units of χ⁽¹⁾, χ⁽²⁾, χ⁽³⁾? | χ⁽¹⁾: dimensionless; χ⁽²⁾: m/V; χ⁽³⁾: m²/V² |
| Why is χ⁽²⁾ = 0 for centrosymmetric materials? | When E → −E, E² → E² (unchanged), but P must reverse. Contradiction → χ⁽²⁾ = 0 |
| What is the atomic field strength E_at? | ≈ 5×10¹¹ V/m (the field an electron experiences in a hydrogen atom) |
| What intensity is required to approach E_at? | ~3×10²⁰ W/m² (from I = ½cε₀E²) |
| Why does doubling wavelength reduce scattering by 16×? | Rayleigh: I ∝ 1/λ⁴; doubling λ → 1/(2λ)⁴ = 1/16 × original |
| What does I ∝ 1/λ⁴ explain about the sky? | Blue light (short λ) scatters more → sky appears blue; at sunset, red light (long λ) reaches us directly |

---

## Polarisation and Timescales

| Question | Answer |
|----------|--------|
| What are the three polarisation timescales? | Electronic: ~10⁻¹⁵ s (femtoseconds); Atomic/vibrational: ~10⁻¹² s (picoseconds); Orientational: ~10⁻⁶ s (microseconds) |
| Why does electronic polarisation NOT give chemical specificity? | It depends only on the length L of the conjugated system, not on the specific chemical bonds |
| Why does atomic/vibrational polarisation give chemical specificity? | The resonant frequency ω_vib = (1/2π)√(k/μ_r) depends on the specific atom masses and bond strength — unique to each bond type |
| What is the reduced mass? | μ_r = m₁m₂/(m₁+m₂) |

---

## Vibrational Spectroscopy

| Question | Answer |
|----------|--------|
| IR selection rule? | The vibration must produce a change in dipole moment (dμ/dQ ≠ 0) |
| Raman selection rule? | The vibration must produce a change in polarizability (dα/dQ ≠ 0) |
| Are these the same? | No — they are complementary; some modes are IR active but not Raman, and vice versa |
| What is a wavenumber (cm⁻¹)? | ν̃ = 1/λ (wavelength in cm) = ν/c; convenient unit for vibrational spectroscopy (0–4000 cm⁻¹) |
| What is a Stokes shift? | Red-shifted Raman line (scattered photon energy lower than incident; molecule gains vibrational energy) |
| Why is IR imaging spatially poor? | Infrared wavelengths (3–10 µm) → diffraction limit d = λ/(2NA) ≈ several µm (much worse than visible) |
| Why is spontaneous Raman too slow for imaging? | ~10⁶ times weaker than fluorescence → 1–10 s per pixel → days for a megapixel image |

---

## Lorentz Oscillator Model

| Question | Answer |
|----------|--------|
| What does ω₀ represent physically? | The natural resonant frequency of the oscillator = √(k/m); determined by the material's restoring force |
| What happens to χ when ω = ω₀? | χ is maximum (resonance); 90° phase lag between E and P |
| What happens to χ at ω ≫ ω₀? | χ → 0 (system cannot respond; 180° out of phase) |
| What assumption breaks down at high fields? | The linear restoring force / parabolic potential — it becomes anharmonic |

---

## Nonlinear Optics

| Question | Answer |
|----------|--------|
| What is SHG? | Second harmonic generation: 2 photons at ω → 1 photon at 2ω. Second-order (χ⁽²⁾) process. |
| What is THG? | Third harmonic generation: 3 photons at ω → 1 photon at 3ω. Third-order (χ⁽³⁾) process. |
| What are the 44 frequency components? | Third-order (χ⁽³⁾) with 3 distinct input frequencies generates up to 44 unique output frequencies |
| What is optical rectification? | The DC term in P⁽²⁾ = ε₀χ⁽²⁾E² — appears when squaring the field, gives a static (ω=0) polarisation |
| What is perturbation theory? | Mathematical technique for solving nonlinear ODEs: expand solution as power series r = λr₁+λ²r₂+…; collect terms at each order of λ |
| What drives the second-order response? | r₁² (the square of the first-order / linear response) |

---

## Phase Matching

| Question | Answer |
|----------|--------|
| Phase matching condition? | k₁ + k₂ = k₃ (or Δk = 0); wave vectors must add up |
| Signal scaling when Δk = 0? | I₃ ∝ L² (signal grows quadratically with interaction length); scales as N² |
| Signal scaling when Δk ≠ 0? | I₃ ∝ sinc²(ΔkL/2) — oscillates rather than grows |
| First zero of sinc²? | When ΔkL/2 = π → ΔkL = 2π → L = 2π/Δk |
| Why does normal dispersion prevent perfect PM? | n(2ω) > n(ω) always → k₃ ≠ k₁+k₂ → Δk ≠ 0 |
| Three phase matching methods? | (1) Angle tuning (birefringence); (2) Temperature tuning; (3) Quasi-PM / periodic poling (PPLN) |
| What is the Gouy phase shift? | π radians of extra phase acquired by a focused Gaussian beam passing through its focal point |
| Why does Gouy phase matter? | It adds to Δk in the microscope: SHG requires L < λ/2; THG requires L < λ/3 |
| Why is THG interface-selective? | L < λ/3 condition cannot be satisfied by bulk material in a tight focus → only interfaces and sub-λ objects contribute |

---

## Laser Pulses

| Question | Answer |
|----------|--------|
| Why pulsed lasers? | NLO scales as Iⁿ (peak intensity). Pulsed operation achieves extreme peak I at moderate average power, avoiding sample damage. |
| Time-bandwidth product for Gaussian pulses? | Δν·Δt ≈ 0.441 |
| What is a transform-limited pulse? | Pulse with the minimum duration for its bandwidth (no excess chirp); achieves the TBP = 0.441 limit |
| What is a chirped pulse? | Pulse where the instantaneous frequency varies across the pulse (due to GVD); red arrives before blue in normal dispersion |
| Which colour arrives first from normal dispersion? | Red (lower frequency → lower refractive index → higher speed → arrives first) |
| 80 MHz vs 1 kHz: same average power, which has higher peak? | 1 kHz — 10⁸× higher peak power (delivers the same energy but in far fewer, longer pulses) |

---

## NLO Microscopy

| Question | Answer |
|----------|--------|
| Why is 2PEF intrinsically confocal? | Signal ∝ I² → only generated where I is very high (at focus) → no out-of-focus signal → no pinhole needed |
| Resolution of 2PEF vs 1PEF (same dye)? | d_2PEF = 0.61√2·λ/NA ≈ 1.41× d_1PEF (not 2×, because of the nonlinear squeeze) |
| Why does 2PEF go deeper than 1PEF? | Excitation at 2λ → Rayleigh scattering 16× less; emitted signal can scatter freely (no pinhole rejection) |
| What biological structures give SHG? | Collagen (in connective tissue, cartilage) and myosin (in muscle) |
| Why? | Both are non-centrosymmetric (χ⁽²⁾ ≠ 0) due to their ordered molecular structure |
| CARS vs SRS: which has no background? | SRS — non-parametric process; electronic (non-resonant) background is absent |
| What laser pulses are needed for CARS/SRS? | Picosecond — to match bandwidth to Raman linewidth (~10–20 cm⁻¹) for spectral selectivity |
| What generates the Stokes beam for CARS? | OPO (Optical Parametric Oscillator) — DFG in a resonant cavity |

---

## Applications

| Question | Answer |
|----------|--------|
| What is virtual H&E? | SRS images (CH₂ for lipids, amide I for proteins) pseudo-coloured to resemble H&E staining; label-free cancer diagnosis |
| What is deuterium labelling? | Replace H with D in drug molecule → shifts C–H stretch (~2950 cm⁻¹) to C–D stretch (~2100 cm⁻¹) in the "silent" region |
| Why does D-labelling work? | m_D ≈ 2m_H → higher reduced mass → lower vibrational frequency → shifts to 2100 cm⁻¹ region; no endogenous biology signals there |
| Why is EPI-CARS selective for nanoparticles? | Backward direction → large Δk → only L < λ/2 objects satisfy phase matching → bulk tissue suppressed; nanoparticles (~100 nm) give signal |
| What is the Raman silent region? | ~1900–2800 cm⁻¹ — no endogenous biological Raman peaks; C–D stretch appears here |
