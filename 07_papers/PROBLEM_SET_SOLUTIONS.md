# Problem Set Solutions

Worked solutions for all four problem sets. For topics already fully covered in `05_exam_prep/`, a brief answer is given with a cross-reference.

---

## Problem Set 1 — Optical Imaging (Lectures 2–3)

### Part I: Image Contrast

**Q1. What is a contrast agent?**
Any substance that, when introduced into a sample, creates a measurable difference in the detected signal between regions of interest and background. Examples: fluorescent dyes, absorbing stains (H&E). A contrast agent makes invisible features visible.

**Q2. Chemical specificity via contrast agents:**
A contrast agent that targets a specific molecular structure (antibody-conjugated dye, HER2 antibody + fluorophore) will label only that target molecule. Spatial distribution of the signal directly maps the target's location → chemical specificity.

**Q3. Why fluorescent labelling fails for small molecules:**
Fluorescent labels (e.g., GFP, fluorescent dyes) are large molecules (MW ~1000 Da). Small molecules such as drugs or metabolites (MW ~100–500 Da) cannot accommodate a label without dramatically altering their chemical behaviour, pharmacokinetics, and biological function. Attaching a bulky fluorophore changes how the molecule diffuses, binds, and is metabolised → the image no longer represents the true distribution of the native molecule.

**Q4. Application requiring chemical specificity without labels:**
Intraoperative cancer margin assessment. During surgery, a pathologist must determine whether the excised tissue has clear margins (cancer-free edges). Exogenous labelling is not possible in real-time during surgery; the sample cannot be fixed and stained without delay. CARS/SRS microscopy provides label-free chemical imaging (lipids, proteins, DNA) to identify cancerous vs normal tissue intraoperatively.

**Q5. Complications of optical absorption as contrast:**
(1) Requires transmitted light → samples must be thin and transparent. (2) Beer-Lambert attenuation means signal depends on sample thickness AND concentration — cannot separate these without knowing path length. (3) Multiple absorbers may overlap spectrally. (4) Scattering masquerades as absorption in thick samples.

### Part II: Spatial Information

**Q6. Define the Rayleigh criterion:**
Two point sources are just resolved when the central maximum of one Airy disc falls on the first minimum of the other. For aperture D and wavelength λ: θ_min = 1.22λ/D.

**Q7. Rayleigh criterion → d = 0.61λ/NA:** See Derivation D04 in `03_master/DERIVATION_BANK.md`.

**Q8. 0.7 NA objective, 532 nm excitation:**
$$d = \frac{0.61 \times 532}{0.7} = \frac{324.5}{0.7} = \textbf{464 nm}$$

**Q9. Gaussian FWHM = 2σ√(2ln2):** See Derivation D03 in `03_master/DERIVATION_BANK.md`.

**Q10. Why immersion media improve resolution:**
NA = n·sinα. Immersion oil (n ≈ 1.515) vs air (n = 1.0) allows the same objective half-angle α to achieve higher NA: NA_oil = 1.515 sinα vs NA_air = sinα. Higher NA → smaller d = 0.61λ/NA → better resolution. Also reduces spherical aberration at the sample interface.

**Q11. Confocal resolution vs depth trade-off:**
Better resolution requires larger NA → larger acceptance angle → shorter working distance → can only image near the surface. In scattering tissue, high-NA excitation focuses poorly at depth (scattered photons destroy the focal spot). To maintain resolution at depth, one must reduce NA (longer working distance) → worse resolution. In practice confocal is limited to ~50–100 µm in tissue before scattering destroys the focal spot quality.

---

## Problem Set 2 — Lorentz Oscillator & Vibrational Spectroscopy (Lectures 4–5)

### Lorentz Oscillator Model

**Q1. Derive χ_e(ω):** See Derivation D01 in `03_master/DERIVATION_BANK.md`.

**Q2. Limitations of the Lorentz oscillator model:**
(1) Assumes a single resonance frequency ω₀ — real materials have multiple electronic transitions at different frequencies. (2) Treats electrons as classical harmonic oscillators — ignores quantum mechanical selection rules and oscillator strengths. (3) Assumes all oscillators are identical (ignores inhomogeneous broadening). (4) Does not account for many-body effects (electron-electron interactions). (5) The damping constant γ is treated as a constant — in reality it is frequency-dependent.

**Q3. Why polarizability is a tensor for non-isotropic materials:**
In an isotropic material, E along x produces P along x. In an anisotropic material (e.g., a crystal), E along x can produce P components along y or z due to the crystal's asymmetric bond arrangement. The relationship P_i = ε₀Σ_j χ_ij E_j requires a 3×3 tensor to capture all possible cross-couplings. Example: birefringent crystals used for phase matching.

**Q4. Amplitude and phase vs wavelength:** See `05_exam_prep/SHORT_ANSWER_BANK.md` (Lorentz Oscillator section) and lecture digest L05.

**Q5. Plasma frequency:**
The frequency ω_p at which the real part of the dielectric function ε₁(ω) = 0. For ω > ω_p, ε₁ > 0 and the material is transparent; for ω < ω_p, ε₁ < 0 and the material is reflective/opaque (metals). Given by ω_p = √(Ne²/mε₀). Metals have ω_p in the UV — hence metallic reflection below UV but transparency above.

### Vibrational Spectroscopy

**Q7. Raman Taylor expansion — induced polarization derivation:**

Polarizability varies with nuclear coordinate Q:
$$\alpha(Q) = \alpha_0 + \left(\frac{d\alpha}{dQ}\right)_0 Q + \ldots$$

The nuclear coordinate oscillates as: Q = Q₀cos(ω_vib t)

Applied electric field: E = E₀cos(ωt)

Induced polarization:
$$P = \varepsilon_0 \alpha(Q) E = \varepsilon_0 \left[\alpha_0 + \left(\frac{d\alpha}{dQ}\right)_0 Q_0\cos(\omega_{vib}t)\right] E_0\cos(\omega t)$$

$$P = \varepsilon_0\alpha_0 E_0\cos(\omega t) + \varepsilon_0\left(\frac{d\alpha}{dQ}\right)_0 Q_0 E_0 \cos(\omega_{vib}t)\cos(\omega t)$$

Using product-to-sum: $\cos A \cos B = \frac{1}{2}[\cos(A-B) + \cos(A+B)]$:

$$\boxed{P = \underbrace{\varepsilon_0\alpha_0 E_0\cos(\omega t)}_{\text{Rayleigh: elastic, } \omega}} + \underbrace{\frac{\varepsilon_0}{2}\left(\frac{d\alpha}{dQ}\right)_0 Q_0 E_0\cos((\omega-\omega_{vib})t)}_{\text{Stokes Raman: } \omega - \omega_{vib}} + \underbrace{\frac{\varepsilon_0}{2}\left(\frac{d\alpha}{dQ}\right)_0 Q_0 E_0\cos((\omega+\omega_{vib})t)}_{\text{Anti-Stokes Raman: } \omega + \omega_{vib}}}$$

Three terms:
1. **Rayleigh**: elastic scattering at ω — most intense
2. **Stokes**: inelastic scattering at ω − ω_vib — molecule gains vibrational energy; red-shifted
3. **Anti-Stokes**: inelastic at ω + ω_vib — molecule loses vibrational energy; blue-shifted; weaker (requires thermally populated vibrational state)

Raman active condition: (dα/dQ)₀ ≠ 0 (change in polarizability during vibration).

**Q8. Spectral regions of vibrational spectrum:**

| Region | Wavenumber | Example motifs |
|--------|-----------|---------------|
| Fingerprint | 500–1800 cm⁻¹ | C-N (~1130), C=C (~1620), C-C, amide I (~1650), amide II (~1550) |
| Silent | 1800–2800 cm⁻¹ | No endogenous biology; C≡C (~2100), C≡N (~2200); C-D stretch (~2100–2300) |
| High wavenumber | 2800–3300 cm⁻¹ | C-H symmetric (~2845), C-H asymmetric (~2930), O-H (~3200), N-H (~3013) |

**Q9. Chemical modifications to shift to silent region:**
(1) **Deuterium labelling**: Replace C-H with C-D. Since m_D ≈ 2m_H, reduced mass increases → ω_vib = (1/2π)√(k/μ_r) decreases. C-H stretch (~2950 cm⁻¹) → C-D stretch (~2100 cm⁻¹), which falls in the silent region.
(2) **¹³C isotope labelling**: Replace ¹²C with ¹³C in specific bonds (e.g., ¹³C=¹³C stretch). Heavier ¹³C increases reduced mass → lower frequency → shifts into or toward the silent region.

**Q10. Advantage over fluorescent labelling:**
These modifications are minimal (replace one atom/isotope). The molecule retains its chemical function, pharmacokinetics, and biological activity. A deuterium-labelled drug tracks exactly like the native drug — unlike a fluorescently labelled drug where the bulky dye (MW ~1000 Da) dominates the molecule's properties. So while not truly label-free, isotope labelling offers near-native tracking of small molecules — something impossible with fluorescent labels.

**Q11. Limitations of linear vibrational spectroscopy for imaging:**
(1) **IR imaging**: spatial resolution limited by IR wavelength (3–10 µm) → only µm-scale features resolved. Aqueous samples absorb strongly in IR → requires dry or thin samples.
(2) **Spontaneous Raman**: signal ~10⁶× weaker than fluorescence → requires long acquisition (seconds per pixel) → days for a megapixel image. Fluorescence background can overwhelm weak Raman signal.
(3) Both require scanning point-by-point → slow for large areas.

---

## Problem Set 3 — NLO Interactions & Ultrafast Pulses (Lectures 7–12)

### Q1: Harmonic oscillator + NL wave equation

Key derivations all in `03_master/DERIVATION_BANK.md`:
- D01: χ(ω) from Lorentz (linear equation of motion)
- D02: SHG χ⁽²⁾ (asymmetric potential, perturbation theory)
- D03: χ⁽²⁾=0 for symmetric (perturbation — no λ² term)
- D07: NL wave equation from Maxwell's equations

### Q2: Phase matching and sinc²

Key derivations in DERIVATION_BANK:
- D08: Coupled amplitude equation (dA₃/dz)
- D09: sinc²(ΔkL/2) from integration

### Q3: Ultrafast laser pulse parameters (3 ps, 1041 nm, 40 MHz, 500 mW)

**(a) Pulse energy:**
$$E_{pulse} = \frac{P_{avg}}{f_{rep}} = \frac{500 \times 10^{-3}}{40 \times 10^6} = \textbf{12.5 nJ}$$

**(b) Optical pathlength between pulses:**
$$\text{Period: } T = \frac{1}{f_{rep}} = \frac{1}{40 \times 10^6} = 25 \text{ ns}$$
$$\text{Path length} = c \times T = 3 \times 10^8 \times 25 \times 10^{-9} = \textbf{7.5 m}$$
This is the total round-trip path length of the laser cavity. For a linear cavity, the physical length is ~3.75 m; for a ring cavity, ~7.5 m. Both are consistent with large Ti:Sapphire systems.

**(c) Peak pulse power:**
$$P_{peak} = \frac{E_{pulse}}{\tau_p} = \frac{12.5 \times 10^{-9}}{3 \times 10^{-12}} = \textbf{4167 W} \approx \textbf{4.2 kW}$$

**(d) Bandwidth:**
$$\Delta\nu = \frac{0.441}{\Delta t} = \frac{0.441}{3 \times 10^{-12}} = 1.47 \times 10^{11} \text{ Hz}$$
$$\Delta\lambda = \frac{\lambda^2}{c}\Delta\nu = \frac{(1041 \times 10^{-9})^2}{3 \times 10^8} \times 1.47 \times 10^{11} = \frac{1.084 \times 10^{-12}}{3 \times 10^8} \times 1.47 \times 10^{11} = \textbf{0.531 nm}$$

In wavenumbers: Δν̃ = 1.47×10¹¹ / 3×10¹⁰ cm/s = **4.9 cm⁻¹**
This is narrower than Raman linewidths (~10–20 cm⁻¹), confirming suitability for CARS.

### Q4: Normal and anomalous dispersion

**Normal dispersion:** Refractive index n increases with frequency (decreases with wavelength): dn/dω > 0. Blue light travels slower than red. Group velocity dispersion (GVD) is positive. A pulse broadens as it propagates — red components arrive first, blue arrive last. Most optical materials (glass, water) show normal dispersion in the visible.

**Anomalous dispersion:** n decreases with increasing frequency: dn/dω < 0. Blue light travels faster than red. GVD is negative. Occurs in some specialty fibres, above the zero-dispersion wavelength of standard silica (~1.3 µm). In anomalous dispersion, soliton propagation (pulse compression) is possible.

**Fourier transform shift theorem:** If f(t) ↔ F(ν), then f(t−t₀) ↔ F(ν)e^{−2πiνt₀}

A time-shift t₀ introduces a linear phase ramp e^{−2πiνt₀} = e^{−iφ(ν)} in the frequency domain, where φ(ν) = 2πνt₀. This is a linear spectral phase. 

Dispersion causes different frequency components to arrive at different times → each frequency component accumulates a different phase → the pulse acquires a non-linear spectral phase → pulse broadens. A chirped pulse has φ(ν) = φ₀ + aν + bν² (quadratic phase = chirp parameter b).

### Q5: Compare 100 fs vs 1 ps pulses (same energy); compare 80 MHz vs 100 kHz at same average power

**100 fs vs 1 ps (same pulse energy E):**
$$\frac{P_{peak,100fs}}{P_{peak,1ps}} = \frac{E/100\times10^{-15}}{E/1\times10^{-12}} = \frac{1\times10^{-12}}{100\times10^{-15}} = \textbf{10×}$$
100 fs pulses have 10× higher peak power for the same energy.

**80 MHz vs 100 kHz (same average power P, same pulse duration 100 fs):**

Pulse energy: E_80MHz = P/80×10⁶; E_100kHz = P/100×10³

$$\frac{E_{100kHz}}{E_{80MHz}} = \frac{80\times10^6}{100\times10^3} = 800$$

Peak power: P_peak = E/τ, so ratio = 800. At the same average power, 100 kHz laser has **800× higher peak power**. At fixed pulse duration, peak intensity ∝ peak power → 100 kHz gives 800× higher intensity.

### Q6: Power required for E_at with 1 NA, 800 nm excitation

FWHM spot: $d = 0.61 \times 800 / 1.0 = 488$ nm → radius r = 244 nm
Area: $A = \pi r^2 = \pi (244 \times 10^{-9})^2 = 1.87 \times 10^{-13}$ m²

Intensity for E_at:
$$I_{at} = \frac{1}{2}c\varepsilon_0 E_{at}^2 = \frac{1}{2}(3\times10^8)(8.85\times10^{-12})(5\times10^{11})^2 = \frac{1}{2} \times 6.64 \times 10^{20} = 3.32 \times 10^{20} \approx 3 \times 10^{20} \text{ W m}^{-2}$$

Required CW power:
$$P_{CW} = I_{at} \times A = 3 \times 10^{20} \times 1.87 \times 10^{-13} = \textbf{5.6 \times 10^7 W} = \textbf{56 MW}$$

This would instantly vaporise any sample and destroy the optics. CW is not viable.

---

## Problem Set 4 — NLO Microscopy & Laser Sources

**Q1. Why NLO removes resolution vs depth trade-off:**
In confocal microscopy, shorter wavelength → better resolution but worse depth penetration (Rayleigh scattering ∝ 1/λ⁴). NLO microscopy uses longer wavelengths (e.g., 800 nm for 2PEF vs 400 nm for 1PEF), dramatically reducing scattering (16× less for 2× wavelength), while achieving similar or better resolution due to the nonlinear PSF squeeze (FWHM ∝ 1/√n for n-photon process). Resolution and depth are no longer coupled through wavelength.

**Q2. Resolution comparison:** See MODEL_QUESTIONS Q9.

**Q3. Tight focus vs collinear beam configurations:**

| Parameter | Tight focus (microscope) | Collinear beams (crystal) |
|-----------|-------------------------|--------------------------|
| Interaction length L | µm scale (focal depth) | mm–cm scale |
| Phase matching | Gouy phase limits L < λ/n; phase matching in bulk is challenging | Requires precise crystal angle/temperature tuning over long L |
| Sectioning | Yes — intrinsic 3D confinement | No |
| Signal scaling | I² over small L | I² over large L → much higher total conversion |
| Applications | Microscopy/imaging | Frequency conversion (SHG in crystals, OPO) |

In tight focus: small interaction volume → lower total conversion, but 3D imaging capability. In collinear: phase matching must be satisfied precisely, but L is large → high-efficiency frequency conversion possible.

**Q4. THG only at interfaces; FWM in bulk:** See `05_exam_prep/SHORT_ANSWER_BANK.md` and PAST_PAPER_SOLUTIONS (Gouy phase section).

**Q5. Optical Parametric Oscillator (OPO):**
An OPO uses DFG (difference frequency generation) in a χ⁽²⁾ crystal inside a resonant optical cavity. A pump beam at ω_p splits into signal (ω_s) and idler (ω_i), where ω_p = ω_s + ω_i and energy conservation is satisfied. The cavity is resonant at ω_s (or sometimes both ω_s and ω_i). By angle or temperature tuning the crystal, ω_s can be continuously varied — providing a tunable laser source.

For CARS microscopy: OPO pumped by 80 MHz Ti:Saph at 800 nm → generates 1040–1200 nm tunable Stokes beam synchronised to the pump → ω_p − ω_s = ω_vib tunable across the fingerprint/CH region.

Energy conservation: 1/λ_p = 1/λ_s + 1/λ_i
