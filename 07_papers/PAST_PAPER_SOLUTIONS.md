# Past Paper Solutions

Worked solutions for question types **not already covered** in `05_exam_prep/MODEL_QUESTIONS.md`. Cross-referenced with new questions Q13–Q20 added to that file.

For solutions to questions that ARE covered, see `05_exam_prep/MODEL_QUESTIONS.md`.

---

## 2023 EXAM — Additional Solutions

### 2023 Q2 (partial) — CW and Pulsed Laser Power for E_at

Already covered in: MODEL_QUESTIONS Q10 (χ estimates) and Q6 (pulse parameters).

**New sub-question: CW power for 1 µm spot at I_at**

Given: I_at = 3×10²⁰ W/m², spot diameter = 1 µm.

Area: A = π(d/2)² = π(0.5×10⁻⁶)² = 7.85×10⁻¹³ m²

P_CW = I × A = 3×10²⁰ × 7.85×10⁻¹³ = **2.36×10⁸ W ≈ 240 MW**

This is catastrophically destructive — any material would vaporise instantly. Confirms CW is not viable.

**New sub-question: Pulsed (100 fs, 1 MHz) average power for the same intensity**

Duty cycle = τ_p × f_rep = 100×10⁻¹⁵ × 1×10⁶ = 10⁻⁷

P_average = P_peak × duty cycle = I × A × duty cycle
= 3×10²⁰ × 7.85×10⁻¹³ × 10⁻⁷
= 2.36×10⁸ × 10⁻⁷
= **23.6 W ≈ 24 W**

Still high for a microscope (typical: 10–100 mW average), but within reach of high-power lasers and far more manageable than 240 MW. This shows why pulsed lasers make NLO microscopy practical.

---

### 2023 Q4 — C-N Bond Calculations (full solution)

**Wavenumber of C-N stretch:**

Force constant: k = 5×10⁵ g s⁻² = 500 N/m (using 1 g s⁻² = 10⁻³ N/m)

Reduced mass:
$$\mu_r = \frac{12 \times 14}{12 + 14} \times 1.66 \times 10^{-27} \text{ kg} = \frac{168}{26} \times 1.66 \times 10^{-27} = 6.46 \times 1.66 \times 10^{-27} = 1.073 \times 10^{-26} \text{ kg}$$

Vibrational frequency:
$$\nu = \frac{1}{2\pi}\sqrt{\frac{k}{\mu_r}} = \frac{1}{2\pi}\sqrt{\frac{500}{1.073 \times 10^{-26}}} = \frac{1}{2\pi} \times 2.159 \times 10^{14} = 3.437 \times 10^{13} \text{ Hz}$$

Wavenumber:
$$\tilde{\nu} = \frac{\nu}{c} = \frac{3.437 \times 10^{13}}{3 \times 10^{10} \text{ cm/s}} = \textbf{1146 cm}^{-1} \approx \textbf{1130 cm}^{-1} \checkmark$$

**IR absorption wavelength:**
$$\lambda_{IR} = \frac{1}{\tilde{\nu}} = \frac{1}{1146 \text{ cm}^{-1}} = 8.73 \times 10^{-4} \text{ cm} = \textbf{8.73 µm}$$

**Stokes Raman wavelength at 514 nm excitation:**

Excitation wavenumber: $\tilde{\nu}_{ex} = \frac{1}{514 \times 10^{-7} \text{ cm}} = 19455 \text{ cm}^{-1}$

Stokes wavenumber: $\tilde{\nu}_S = 19455 - 1146 = 18309 \text{ cm}^{-1}$

Stokes wavelength:
$$\lambda_S = \frac{1}{18309 \text{ cm}^{-1}} = 5.46 \times 10^{-5} \text{ cm} = \textbf{546 nm}$$

---

## 2024 EXAM — Additional Solutions

### 2024 Q1 — Chemical Specificity and Labelling Limitations

**Why electronic absorption does not provide chemical information:**
Electronic transitions depend on the conjugation length L (via the infinite square well: E ∝ 1/L²). They do NOT depend on the specific chemical bonds — two molecules with the same length conjugated system absorb at the same wavelength even if the atoms differ. Therefore colour = conjugation length, not chemical identity.

**Why vibrational resonances provide chemical information:**
Vibrational frequency ω_vib = (1/2π)√(k/μ_r) depends on both the bond spring constant k AND the reduced mass μ_r = m₁m₂/(m₁+m₂). These are unique to each bond type (C-H at ~2950 cm⁻¹, C=O at ~1750 cm⁻¹, C-N at ~1130 cm⁻¹). The vibrational spectrum is a molecular fingerprint.

**How CRS overcomes weak spontaneous Raman:**
- Coherent driving: CARS/SRS use pump + Stokes beams tuned to ω_p − ω_s = ω_vib, coherently driving all molecules in the focal volume in phase → signal scales as N² rather than N (constructive interference of N emitters)
- Signal level 10⁵–10⁷× higher than spontaneous Raman → enables video-rate imaging

### 2024 Q2 — Infinite Square Well: Molecule Size for 500 nm Absorption

**Physical context:** Atomic hydrogen absorbs at 122 nm (Lyman-α); the model predicts E = −13.6/n² eV, so ΔE(1→2) = 10.2 eV. This is far UV, not visible. Conjugated molecules absorb in the visible because electrons are delocalised over many bond lengths.

**Calculation:**

Energy levels of infinite square well: $E_n = \frac{n^2 \pi^2 \hbar^2}{8 m_e L^2}$

Transition from ground (n=1) to first excited state (n=2):
$$\Delta E = E_2 - E_1 = \frac{(4-1)\pi^2\hbar^2}{8m_e L^2} = \frac{3\pi^2\hbar^2}{8m_e L^2}$$

Set equal to photon energy for λ = 500 nm:
$$\frac{3\pi^2\hbar^2}{8m_e L^2} = \frac{hc}{\lambda}$$

Solve for L²:
$$L^2 = \frac{3\pi^2\hbar^2\lambda}{8m_e hc}$$

Note: ℏ = h/2π → ℏ² = h²/4π², so:
$$L^2 = \frac{3h^2\lambda}{32m_e c} = \frac{3 \times (6.626 \times 10^{-34})^2 \times 500 \times 10^{-9}}{32 \times 9.109 \times 10^{-31} \times 6.626 \times 10^{-34} \times 3 \times 10^8}$$

Numerator: 3 × 4.390×10⁻⁶⁷ × 5×10⁻⁷ = 6.585×10⁻⁷³

Denominator: 32 × 9.109×10⁻³¹ × 6.626×10⁻³⁴ × 3×10⁸ = 32 × 1.811×10⁻⁵⁶ = 5.796×10⁻⁵⁵

L² = 6.585×10⁻⁷³ / 5.796×10⁻⁵⁵ = 1.136×10⁻¹⁸ m²

Wait — let me redo carefully with ℏ directly:

$$L^2 = \frac{3\pi^2\hbar^2\lambda}{8m_e hc}$$

= (3 × 9.870 × (1.055×10⁻³⁴)² × 500×10⁻⁹) / (8 × 9.109×10⁻³¹ × 6.626×10⁻³⁴ × 3×10⁸)

Numerator: 3 × 9.870 × 1.113×10⁻⁶⁸ × 5×10⁻⁷ = 1.648×10⁻⁷³

Denominator: 8 × 9.109×10⁻³¹ × 6.626×10⁻³⁴ × 3×10⁸ = 1.449×10⁻⁵⁴

$$L^2 = \frac{1.648 \times 10^{-73}}{1.449 \times 10^{-54}} = 1.137 \times 10^{-19} \text{ m}^2$$

$$\boxed{L = \sqrt{1.137 \times 10^{-19}} = 3.37 \times 10^{-10} \text{ m} \approx 0.34 \text{ nm}}$$

This is the length scale of a benzene ring (~0.28 nm) or a short conjugated chain (3–5 alternating C=C bonds). A conjugated π system with ~3 double bonds absorbs at ~500 nm.

**The example to give:** A conjugated π system / aromatic ring such as benzene or a short polyene.

---

### 2024 Q3 — Ti:Saph Pulse Parameters (120 fs, 900 nm, 40 MHz, 10 mW, 1 µm spot)

**(a) Pulse energy:**
$$E_{pulse} = \frac{P_{avg}}{f_{rep}} = \frac{10 \times 10^{-3}}{40 \times 10^6} = 2.5 \times 10^{-10} \text{ J} = \textbf{0.25 nJ}$$

**(b) Peak power:**
$$P_{peak} = \frac{E_{pulse}}{\tau_p} = \frac{2.5 \times 10^{-10}}{120 \times 10^{-15}} = \textbf{2083 W} \approx \textbf{2.1 kW}$$

**(c) Peak intensity (1 µm diameter spot → r = 0.5 µm):**
$$A = \pi r^2 = \pi (0.5 \times 10^{-6})^2 = 7.85 \times 10^{-13} \text{ m}^2$$
$$I_{peak} = \frac{P_{peak}}{A} = \frac{2083}{7.85 \times 10^{-13}} = \textbf{2.65 \times 10^{15} \text{ W m}^{-2}}$$

**(d) Bandwidth in nm (using TBP):**
$$\Delta\nu = \frac{0.441}{\Delta t} = \frac{0.441}{120 \times 10^{-15}} = 3.675 \times 10^{12} \text{ Hz}$$
$$\Delta\lambda = \frac{\lambda^2}{c}\Delta\nu = \frac{(900 \times 10^{-9})^2}{3 \times 10^8} \times 3.675 \times 10^{12} = \frac{8.1 \times 10^{-13}}{3 \times 10^8} \times 3.675 \times 10^{12} = \textbf{9.9 \text{ nm}}$$

### 2024 Q3 — Kerr-Lens Mode Locking (KLM) [6 marks]

**Key points to cover:**

1. **Kerr effect**: In a nonlinear medium (Ti:Sapphire crystal itself), the refractive index depends on intensity: n = n₀ + n₂I. For a Gaussian beam profile, the centre of the beam sees higher intensity than the edges → higher refractive index at the centre → the medium acts as a positive lens (the Kerr lens).

2. **Self-focusing**: This intensity-dependent lensing focuses high-intensity pulses more tightly than low-intensity CW radiation. A pulsed beam creates a tighter focal spot than a CW beam of the same average power.

3. **Selection mechanism**: An aperture (hard aperture or soft aperture from the gain medium itself) is placed in the cavity such that the tightly focused pulsed mode couples more efficiently through it than the CW mode. This preferentially amplifies pulsed operation.

4. **Starting**: KLM is not self-starting (unlike SESAM). The laser requires a perturbation (physical bump to a mirror, acoustic vibration) to initiate pulsing. Once a short pulse exists, the Kerr lens sustains it.

5. **Result**: Mode-locked Ti:Sapphire typically produces 10–150 fs pulses at 80 MHz repetition rate, with bandwidth spanning ~100 nm centred at ~800 nm.

**Sketch required:** Show intensity profile of beam cross-section → refractive index profile (higher at centre) → converging lens effect → tight focus through aperture.

---

### 2024 Q4 — Nonlinear Wave Equation from Maxwell's (6 marks)

**See Derivation Bank D07** in `03_master/DERIVATION_BANK.md` for the complete derivation. Summary of steps for exam:

1. Start: ∇×H = ∂D/∂t (no free currents); ∇×E = −∂B/∂t
2. Take curl of Faraday: ∇×(∇×E) = −∂/∂t(∇×B) = −μ₀∂²D/∂t²
3. Apply vector identity: ∇×(∇×E) = ∇(∇·E) − ∇²E → ≈ −∇²E (using ∇·E ≈ 0)
4. Split D = ε₀n²E + P_NL
5. Result: ∇²E − (n²/c²)∂²E/∂t² = (1/ε₀c²)∂²P_NL/∂t²

The RHS is the source term driven by P_NL — the nonlinear polarization radiates at new frequencies.

---

### 2025 EXAM — Additional Solutions

### 2025 Q1 — Hydrogen Atom → No Visible Contrast [2 marks]

Energy levels of hydrogen: $E_n = -13.6 Z^2/n^2$ eV (Z=1 for hydrogen)

Ground state: E₁ = −13.6 eV; First excited state: E₂ = −3.4 eV

ΔE = 10.2 eV

Corresponding wavelength:
$$\lambda = \frac{hc}{\Delta E} = \frac{(4.136 \times 10^{-15} \text{ eV·s})(3 \times 10^8 \text{ m/s})}{10.2 \text{ eV}} = \frac{1.241 \times 10^{-6} \text{ eV·m}}{10.2 \text{ eV}} = 122 \text{ nm}$$

This is deep ultraviolet (Lyman-α), far below the visible range (400–700 nm). Atomic electronic transitions cannot provide visible contrast because the energy gaps are too large.

### 2025 Q1 — N-H Bond IR Wavelength and Raman Stokes [3+2 marks]

**IR absorption wavelength:**

k = 5×10⁵ g s⁻² = 500 N/m

Reduced mass: $\mu_r = \frac{14 \times 1}{14 + 1} \times 1.66 \times 10^{-27} = \frac{14}{15} \times 1.66 \times 10^{-27} = 1.549 \times 10^{-27}$ kg

Vibrational frequency:
$$\nu = \frac{1}{2\pi}\sqrt{\frac{500}{1.549 \times 10^{-27}}} = \frac{1}{2\pi} \times 5.68 \times 10^{14} = 9.04 \times 10^{13} \text{ Hz}$$

Wavenumber: $\tilde{\nu} = 9.04 \times 10^{13} / 3 \times 10^{10} = 3013$ cm⁻¹

IR wavelength: $\lambda_{IR} = 1/3013 \text{ cm}^{-1} = 3.32 \times 10^{-4}$ cm = **3.32 µm**

**Stokes Raman wavelength at 785 nm excitation:**

Excitation wavenumber: $\tilde{\nu}_{ex} = 1/(785 \times 10^{-7} \text{ cm}) = 12739$ cm⁻¹

Stokes wavenumber: $\tilde{\nu}_S = 12739 - 3013 = 9726$ cm⁻¹

Stokes wavelength: $\lambda_S = 1/9726 = 1.028 \times 10^{-4}$ cm = **1028 nm ≈ 1.03 µm**

### 2025 Q2 — Resolution at 532 nm and 1064 nm [2,2 marks]

**At 532 nm, NA = 1.2:**
$$d_{532} = \frac{0.61 \times 532}{1.2} = \frac{324.5}{1.2} = \textbf{271 nm}$$

**At 1064 nm, NA = 1.2:**
$$d_{1064} = \frac{0.61 \times 1064}{1.2} = \frac{649}{1.2} = \textbf{541 nm}$$

### 2025 Q2 — Rayleigh Scattering Ratio (532 vs 1064 nm) [2 marks]

Rayleigh scattering intensity: I ∝ 1/λ⁴

$$\frac{I_{532}}{I_{1064}} = \left(\frac{\lambda_{1064}}{\lambda_{532}}\right)^4 = \left(\frac{1064}{532}\right)^4 = 2^4 = \textbf{16}$$

Scattering at 532 nm is **16× stronger** than at 1064 nm. This is why NLO microscopy using 1064 nm penetrates much deeper than confocal using 532 nm.

### 2025 Q2 — 2nd and 3rd Order NLO Resolution at 1064 nm [3,3 marks]

**Second-order NLO (e.g., SHG) at 1064 nm:**

Linear FWHM at 1064 nm: d_lin = 0.61×1064/1.2 = 541 nm

For a second-order process, signal ∝ I², so the effective PSF is I². The FWHM of I²(r) where I(r) ∝ exp(−r²/σ²):
$$I^2(r) \propto \exp\left(-\frac{2r^2}{\sigma^2}\right) \rightarrow \sigma_{eff} = \sigma/\sqrt{2}$$

FWHM scales as 1/√2:
$$d_{2nd} = \frac{d_{lin}}{\sqrt{2}} = \frac{541}{\sqrt{2}} = \textbf{382 nm}$$

**Third-order NLO (e.g., THG) at 1064 nm:**

Signal ∝ I³: FWHM scales as 1/√3:
$$d_{3rd} = \frac{d_{lin}}{\sqrt{3}} = \frac{541}{\sqrt{3}} = \textbf{312 nm}$$

**Comparison:** The 1064 nm NLO resolution (382 nm for 2nd order) is notably worse than single-photon 532 nm (271 nm), but the depth advantage (16× less scattering) far outweighs the resolution penalty for imaging in thick tissue.

### 2025 Q2 — Phase Matching: Why Normal Dispersion Prevents It (SFG example) [3 marks]

**Phase matching condition for SFG (ω₃ = ω₁ + ω₂):**
$$k_3 = k_1 + k_2 \quad \Leftrightarrow \quad n_3\omega_3 = n_1\omega_1 + n_2\omega_2$$

For SFG where ω₃ > ω₁ and ω₃ > ω₂:

In a normal dispersive material, refractive index **increases with frequency** (decreases with wavelength): n(ω₃) > n(ω₁) and n(ω₃) > n(ω₂).

Substituting ω₃ = ω₁ + ω₂:
$$n_3(\omega_1 + \omega_2) \neq n_1\omega_1 + n_2\omega_2 \text{ in general}$$

Because n₃ > n₁, n₂, the generated field (k₃) walks ahead of the driving polarization (k₁+k₂), building up phase mismatch. Δk = k₃ − k₁ − k₂ > 0 → the sinc²(ΔkL/2) suppresses the signal.

**Solutions:** Birefringence (use ordinary/extraordinary indices at different angles), temperature tuning, or quasi-phase-matching (PPLN periodic poling).

### 2025 Q2 — Gouy Phase: FWM Bulk vs THG Interface [2 marks]

A Gaussian beam acquires a total phase shift of π as it passes through its focal waist (the Gouy phase).

**For THG (ω → 3ω, third-harmonic):**
The nonlinear polarization P⁽³⁾ ∝ E³. Each input photon contributes its Gouy phase, giving P⁽³⁾ a net accumulated Gouy phase of 3×π/2... 

More precisely: the driving polarization P⁽³⁾ ∝ E³ acquires 3 times the Gouy phase of the fundamental, while the generated harmonic field at 3ω acquires only its own Gouy phase (π). The net mismatch = 3π − π = 2π. This corresponds to an effective Δk × L = 2π, restricting efficient THG to interaction lengths L < λ/3. No bulk material satisfies this in a tight focus → THG only at interfaces or sub-λ objects.

**For FWM/CARS (pump × pump × Stokes* → anti-Stokes):**
The driving polarization P⁽³⁾ ∝ E_p² × E_s*. The conjugate E_s* contributes a **negative** Gouy phase. Net Gouy phase on P⁽³⁾ = π + π − π = π. The generated anti-Stokes acquires +π from its own Gouy phase. Net mismatch = π − π = 0. FWM is therefore Gouy-phase-matched in the forward direction → generates signal from bulk material.

### 2025 Q4 — Precise χ⁽³⁾ = 3.78×10⁻²⁴ m²/V² [4+3 marks]

**Calculate E_at precisely:**

Using Bohr radius: $a_0 = 5.29 \times 10^{-11}$ m, charge e = 1.6×10⁻¹⁹ C

$$E_{at} = \frac{e}{4\pi\varepsilon_0 a_0^2} = \frac{1.6 \times 10^{-19}}{4\pi \times 8.85 \times 10^{-12} \times (5.29 \times 10^{-11})^2}$$

Denominator: 4π × 8.85×10⁻¹² × 2.798×10⁻²¹ = 3.116×10⁻³¹

$$E_{at} = \frac{1.6 \times 10^{-19}}{3.116 \times 10^{-31}} = 5.14 \times 10^{11} \text{ V/m}$$

(The 2025 paper uses this more precise value — the 2023/2024 papers round to 5×10¹¹ V/m.)

**Derive χ⁽³⁾:**

At E = E_at, third-order polarization equals linear polarization:
$$\varepsilon_0\chi^{(1)}E_{at} = \varepsilon_0\chi^{(3)}E_{at}^3$$
$$\chi^{(3)} = \frac{\chi^{(1)}}{E_{at}^2} \approx \frac{1}{(5.14 \times 10^{11})^2} = \frac{1}{2.642 \times 10^{23}} = 3.78 \times 10^{-24} \text{ m}^2/\text{V}^2 \checkmark$$

### 2025 Q4 — CARS Pulse Parameters (1 ps, 1064 nm, 80 MHz, 10 mW) [2+2+2 marks]

**Pulse energy:**
$$E_{pulse} = \frac{P_{avg}}{f_{rep}} = \frac{10 \times 10^{-3}}{80 \times 10^6} = 1.25 \times 10^{-10} \text{ J} = \textbf{0.125 nJ}$$

**Peak power:**
$$P_{peak} = \frac{E_{pulse}}{\tau_p} = \frac{1.25 \times 10^{-10}}{1 \times 10^{-12}} = \textbf{125 W}$$

**Pulse bandwidth in microns:**

Using TBP:
$$\Delta\nu = \frac{0.441}{\Delta t} = \frac{0.441}{1 \times 10^{-12}} = 4.41 \times 10^{11} \text{ Hz}$$

Convert to wavelength:
$$\Delta\lambda = \frac{\lambda^2}{c}\Delta\nu = \frac{(1064 \times 10^{-9})^2}{3 \times 10^8} \times 4.41 \times 10^{11}$$
$$= \frac{1.132 \times 10^{-12}}{3 \times 10^8} \times 4.41 \times 10^{11} = 3.773 \times 10^{-21} \times 4.41 \times 10^{11} = 1.66 \times 10^{-9} \text{ m}$$

$$\Delta\lambda = \textbf{1.66 nm} = 0.00166 \text{ µm}$$

In wavenumbers: Δν̃ = 4.41×10¹¹ / (3×10¹⁰ cm/s) = **14.7 cm⁻¹**

**Why this matches CARS:** Spontaneous Raman linewidths are ~10–20 cm⁻¹. With 1 ps pulses (14.7 cm⁻¹ bandwidth), the excitation bandwidth matches the Raman line → maximum selectivity and contrast. Femtosecond pulses (~100 fs) would have ~150 cm⁻¹ bandwidth, exciting many Raman lines simultaneously → loss of chemical selectivity and increased non-resonant background.

### 2025 Q4 — Saturable Absorber (SESAM) Band Diagrams [2+3 marks]

**Saturable absorption band diagram (2 marks):**
- Two-level system: valence band (ground) and conduction band (excited)
- Low intensity: many available states → photon absorbed (high loss)
- High intensity: states fill up (Pauli exclusion) → absorption saturates → low loss
- Show: bands at equilibrium with empty conduction band. Then under high I: conduction band filled, absorption bleached.

**Time-dependent power loss and gain in cavity (3 marks):**
- Sketch: x-axis = time, y-axis = optical power
- Initially: round-trip gain = round-trip loss (CW threshold)
- Gain medium has slow gain recovery (microsecond timescale)
- SESAM has fast absorption recovery (picosecond timescale)
- For a short pulse: SESAM bleaches fast (during pulse) → net loss drops → gain > loss → pulse amplified
- After pulse: gain recovers slowly → next pulse amplified
- Key feature: the fast-recovering absorber preferentially passes short pulses → mode-locking
- Draw the characteristic shape: gain (slow, approximately flat during pulse), loss (fast dip and recovery), power pulse (narrow spike)
