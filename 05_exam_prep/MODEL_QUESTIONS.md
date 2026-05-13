# Model Questions

Exam-style questions with worked solutions. Based on the style of questions described and demonstrated in lectures.

---

## Section A: Short Derivations and Explanations

### Q1 — Lorentz Oscillator Derivation

**Question:** Derive an expression for the linear electric susceptibility χ⁽¹⁾(ω) for a dielectric material using the Lorentz oscillator model. State the physical meaning of each term in the equation of motion.

**Solution:** See Derivation D01 in `DERIVATION_BANK.md`.

Key result: χ⁽¹⁾(ω) = [Nq²/(mε₀)] / [(ω₀²−ω²) − iγω]

Sketch of χ vs ω: DC plateau, resonance peak at ω₀, fall-off at high ω.

---

### Q2 — Centrosymmetry

**Question:** Explain why materials with a centre of symmetry exhibit χ⁽²⁾ = 0. Sketch two potentials — one centrosymmetric, one not — and explain how each responds to a single-frequency sinusoidal driving field.

**Solution:**
For centrosymmetric material: when E → −E, the displacement P⁽²⁾ = ε₀χ⁽²⁾E² is unchanged (E² is always positive), but a physical displacement must reverse direction when E reverses. This contradiction requires χ⁽²⁾ = 0.

Non-centrosymmetric potential: asymmetric top/bottom → distorted output waveform (peaky on one side) → contains even harmonics (2ω). 
Centrosymmetric potential: symmetric → output waveform distorted but symmetrically → contains only odd harmonics (3ω).

---

### Q3 — Bandwidth Calculation

**Question:** A mode-locked Ti:Sapphire laser produces transform-limited Gaussian pulses of duration 150 fs centred at 800 nm. Calculate: (a) the bandwidth in frequency; (b) the bandwidth in wavelength.

**Solution:**

(a) Using time-bandwidth product Δν·Δt = 0.441:
$$\Delta\nu = \frac{0.441}{\Delta t} = \frac{0.441}{150\times10^{-15}} = 2.94\times10^{12} \text{ Hz} = 2.94 \text{ THz}$$

(b) Convert to wavelength using Δλ = (λ²/c)Δν:
$$\Delta\lambda = \frac{(800\times10^{-9})^2}{3\times10^8} \times 2.94\times10^{12} = \frac{6.4\times10^{-13}}{3\times10^8} \times 2.94\times10^{12}$$
$$= 2.13\times10^{-21} \times 2.94\times10^{12} = 6.3\times10^{-9} \text{ m} \approx 6.3 \text{ nm}$$

---

### Q4 — Rayleigh Criterion Derivation

**Question:** Show that the angular Rayleigh criterion θ_min = 1.22λ/D can be expressed as a minimum resolvable distance d_min = 0.61λ/NA for a microscope objective.

**Solution:** See Derivation D04 in `DERIVATION_BANK.md`.

---

### Q5 — Confocal Scattering Limitation

**Question:** Explain why Rayleigh scattering limits the depth penetration of confocal fluorescence microscopy, even though scattering should *increase* the collection efficiency by redirecting more photons toward the detector.

**Solution:**
The confocal detection pinhole requires emitted photons to arrive at a very specific position (the confocal point). Photons that undergo even one scattering event are redirected and arrive at the *wrong position* at the pinhole plane → they are rejected. While scattering does increase the total number of photons emitted, the photons that matter (from the focal plane) are being lost by scattering events before reaching the pinhole.

To compensate, the excitation laser power must be increased, but this risks photodamage.

---

## Section B: Calculations

### Q6 — Pulse Parameters

**Question:** A 80 MHz mode-locked laser has an average output power of 500 mW and a pulse duration of 100 fs. The beam is focused to a spot radius of 1 µm at the sample.  
Calculate: (a) pulse energy; (b) peak power; (c) peak intensity.

**Solution:**

(a) E_pulse = P_av / f_rep = 500×10⁻³ / (80×10⁶) = **6.25×10⁻⁹ J = 6.25 nJ**

(b) P_peak = E_pulse / τ_p = 6.25×10⁻⁹ / (100×10⁻¹⁵) = **6.25×10⁴ W = 62.5 kW**

(c) Area: A = π×(1×10⁻⁶)² = 3.14×10⁻¹² m²

I_peak = P_peak / A = 6.25×10⁴ / (3.14×10⁻¹²) = **2.0×10¹⁶ W m⁻²**

---

### Q7 — CARS Wavelength Calculation

**Question:** A CARS microscope uses a 1040 nm pump laser. Determine: (a) the Stokes laser wavelength needed to probe the C–H₂ symmetric stretch at 2845 cm⁻¹; (b) the wavelength of the detected anti-Stokes signal.

**Solution:**

Convert all wavelengths to cm:
λ_P = 1040 nm = 1040×10⁻⁷ cm = 1.04×10⁻⁴ cm
1/λ_P = 9615 cm⁻¹

(a) Stokes: 1/λ_S = 1/λ_P − ν̃_vib = 9615 − 2845 = 6770 cm⁻¹
λ_S = 1/6770 cm = 1.477×10⁻⁴ cm = **1477 nm**

(b) Anti-Stokes: 1/λ_AS = 1/λ_P + ν̃_vib = 9615 + 2845 = 12460 cm⁻¹
λ_AS = 1/12460 cm = 8.03×10⁻⁵ cm = **803 nm**

Sanity check: λ_S > λ_P (1477 > 1040) ✓; λ_AS < λ_P (803 < 1040) ✓

---

### Q8 — Vibrational Frequency Calculation

**Question:** Calculate the expected wavenumber of the N–H stretching vibration. Atomic masses: N = 14 u, H = 1 u. Use a spring constant appropriate for a single bond (k ≈ 5×10² N/m).

**Solution:**

Reduced mass: μ_r = (14 × 1)/(14 + 1) × 1.66×10⁻²⁷ kg = 0.933 × 1.66×10⁻²⁷ = 1.55×10⁻²⁷ kg

Vibrational frequency:
$$\nu_{vib} = \frac{1}{2\pi}\sqrt{\frac{k}{\mu_r}} = \frac{1}{2\pi}\sqrt{\frac{500}{1.55\times10^{-27}}} = \frac{1}{2\pi}\times5.68\times10^{14} = 9.04\times10^{13} \text{ Hz}$$

Wavenumber: ν̃ = ν/c = 9.04×10¹³ / (3×10¹⁰ cm/s) = **3013 cm⁻¹**

(Actual N–H stretch is ~3300–3500 cm⁻¹; the single-bond spring constant is approximate.)

---

### Q9 — Resolution Comparison

**Question:** A fluorescent dye has excitation peak at 400 nm. Compare the theoretical spatial resolution achievable with a NA = 1.2 objective using: (a) single-photon confocal excitation at 400 nm; (b) two-photon excitation at 800 nm; (c) three-photon excitation at 1200 nm.

**Solution:**

(a) 1PEF: d₁ = 0.61 × 400 / 1.2 = **203 nm**

(b) 2PEF: First calculate as if linear: 0.61 × 800 / 1.2 = 407 nm; apply nonlinear squeeze: 407 / √2 = **288 nm**

(c) 3PEF: 0.61 × 1200 / 1.2 = 610 nm; apply squeeze: 610 / √3 = **352 nm**

The 1PEF gives the best theoretical resolution but cannot achieve this in scattering tissue beyond ~50 µm. 2PEF achieves 288 nm to ~800 µm depth.

---

### Q10 — χ Estimates

**Question:** Using the assumption that nonlinear susceptibilities become comparable to the linear susceptibility when the applied field E ≈ E_at (the atomic field strength), estimate χ⁽²⁾ and χ⁽³⁾, giving their units.

**Solution:**

E_at ≈ 5×10¹¹ V/m; χ⁽¹⁾ ≈ 1 (dimensionless, solid-state material)

At E = E_at: χ⁽¹⁾E_at ≈ χ⁽²⁾E_at² → χ⁽²⁾ ≈ χ⁽¹⁾/E_at = 1/(5×10¹¹) ≈ **2×10⁻¹² m/V**

Similarly: χ⁽³⁾ ≈ χ⁽¹⁾/E_at² = 1/(5×10¹¹)² ≈ **4×10⁻²⁴ m²/V²**

Units: χ⁽²⁾ in m/V (one extra factor of E in denominator); χ⁽³⁾ in m²/V² (two extra factors).

---

## Section C: Extended Discussions

### Q11 — Explain how 2PEF overcomes the three main limitations of confocal fluorescence microscopy

**Model answer (structured for exam):**

**Limitation 1: Labels required**  
2PEF still requires fluorescent labels for fluorescence imaging. However, it enables complementary label-free techniques (SHG for collagen/myosin, CARS/SRS for molecular fingerprint). So this limitation is partially addressed.

**Limitation 2: Scattering defeats pinhole**  
2PEF signal scales as I². The high intensity only exists at the focal point, so signal is **only generated** at the focal volume regardless of how scattered the emitted photons become. We can place a large-area detector and collect all the scattered emitted photons — we don't need a pinhole. This completely removes the scattering-kills-confocal limitation.

**Limitation 3: Short wavelength vs. deep penetration tradeoff**  
2PEF excites a 400 nm dye using 800 nm light (2× wavelength). Rayleigh scattering of 800 nm excitation is 16× less than 400 nm (factor of 2⁴). This dramatically increases the depth at which the excitation can create a clean focal spot. Additionally, because we don't need a pinhole for detection, any emitted photons that scatter on their way out can still be collected. Typical depth: ~800 µm in brain vs. ~50–100 µm for confocal.

**Summary:** 2PEF achieves intrinsic 3D confinement (advantage 1), eliminates scattering-induced pinhole loss (advantage 2), and uses longer excitation wavelengths to penetrate deeper (advantage 3).

---

### Q12 — Phase matching in CARS and EPI-CARS

**Question:** Explain, using the phase matching derivation, why forward-detected CARS gives signal from bulk material while backward (EPI) CARS is selective for sub-wavelength structures.

**Model answer:**

**Forward CARS:** The signal frequency ω_AS = 2ω_P − ω_S propagates in the same direction as the input beams. The phase mismatch Δk = k_AS − 2k_P + k_S is small (because the refractive indices at these three closely-spaced frequencies are similar). The sinc²(ΔkL/2) condition is satisfied for macroscopic interaction lengths → bulk material generates strong forward CARS.

**Backward (EPI) CARS:** The signal propagates backwards, so k_AS is reversed: Δk_eff = −k_AS − 2k_P + k_S = −2k_AS (roughly). This is very large — approximately 4k_P/c × n. The sinc²(ΔkL/2) = 0 unless L < π/Δk_eff ≈ λ_P/(2n). This is sub-wavelength. So only objects smaller than approximately λ/2 can satisfy this condition and generate backwards CARS. Bulk material (L >> λ) gives no backwards signal because the front and back half of the focal volume contribute anti-phase.

---

## Section D: Questions from Real Past Papers (2023–2025)

*These question types appear in official past papers but were not in the original model question set. Full worked solutions are in `07_papers/PAST_PAPER_SOLUTIONS.md`.*

### Q13 — Infinite Square Well: Molecule Size for Visible Absorption
*(2024 Q2 [3 marks]; 2025 Q1 [2 marks])*

**Question:** Using the 1D infinite square well as a model, estimate the minimum length of a conjugated molecule that absorbs at 500 nm.

**Solution:**

Energy levels: $E_n = \frac{n^2\pi^2\hbar^2}{8m_e L^2}$

Ground→first excited state (n=1→2):
$$\Delta E = \frac{3\pi^2\hbar^2}{8m_e L^2} = \frac{hc}{\lambda}$$

Solve for L:
$$L^2 = \frac{3\pi^2\hbar^2\lambda}{8m_e hc} = \frac{3 \times 9.870 \times (1.055\times10^{-34})^2 \times 500\times10^{-9}}{8 \times 9.109\times10^{-31} \times 6.626\times10^{-34} \times 3\times10^8}$$

$$L^2 = \frac{1.648\times10^{-73}}{1.449\times10^{-54}} = 1.14\times10^{-19} \text{ m}^2 \implies \boxed{L \approx 0.34 \text{ nm}}$$

This is the scale of a benzene ring or a short conjugated chain (~3–5 C=C double bonds).

---

### Q14 — Hydrogen Atom → No Visible Absorption
*(2025 Q1 [2 marks])*

**Question:** Show that electronic absorption in atomic hydrogen does not produce contrast in the visible wavelength range.

**Solution:**

$$E_n = -\frac{13.6}{n^2} \text{ eV} \quad (Z = 1)$$

$$\Delta E_{1\to2} = E_2 - E_1 = -3.4 - (-13.6) = 10.2 \text{ eV}$$

$$\lambda = \frac{hc}{\Delta E} = \frac{1.241\times10^{-6} \text{ eV·m}}{10.2 \text{ eV}} = \textbf{122 nm (UV)}$$

This is deep ultraviolet — far below the visible range (400–700 nm). Atomic transitions cannot produce visible optical contrast.

**Follow-up:** Conjugated molecules use the square well model with L ~ nm scale → ΔE drops into the visible range. The colour of a dye is determined by its conjugation length, not its chemical identity.

---

### Q15 — CW vs Pulsed Laser Power for E_at
*(2023 Q2 [3+4 marks])*

**Question:** For NLO microscopy with a 1 µm diameter spot, (a) calculate the average power required for a CW laser to achieve I_at = 3×10²⁰ W/m². (b) Calculate the average power required using 100 fs pulses at 1 MHz repetition rate.

**Solution:**

Area: A = π(0.5×10⁻⁶)² = 7.85×10⁻¹³ m²

**(a) CW:**
$$P_{CW} = I_{at} \times A = 3\times10^{20} \times 7.85\times10^{-13} = \textbf{240 MW}$$
Completely impractical — would instantly vaporise any sample.

**(b) 100 fs pulses at 1 MHz:**

Duty cycle = τ_p × f_rep = 100×10⁻¹⁵ × 10⁶ = 10⁻⁷

$$P_{avg} = I_{at} \times A \times \text{duty cycle} = 240\times10^6 \times 10^{-7} = \textbf{24 W}$$

Still high for a microscope (typical: 1–100 mW), but achievable. Pulsed operation makes NLO microscopy physically possible.

---

### Q16 — Stokes Wavelength and IR Wavelength Calculation
*(2023 Q4 [2+2]; 2025 Q1 [2+3])*

**Question:** For a 785 nm excitation laser and the N-H stretching vibration (k = 500 N/m): (a) calculate the IR absorption wavelength; (b) calculate the Stokes Raman wavelength.

**Solution:**

Reduced mass: $\mu_r = \frac{14\times1}{15}\times1.66\times10^{-27} = 1.549\times10^{-27}$ kg

Wavenumber: $\tilde{\nu}_{NH} = \frac{1}{2\pi c}\sqrt{\frac{k}{\mu_r}} = \frac{5.68\times10^{14}}{2\pi\times3\times10^{10}} = 3013$ cm⁻¹

**(a) IR wavelength:**
$$\lambda_{IR} = \frac{1}{3013 \text{ cm}^{-1}} = 3.32\times10^{-4} \text{ cm} = \textbf{3.32 µm}$$

**(b) Stokes Raman at 785 nm:**

$$\tilde{\nu}_{ex} = \frac{1}{785\times10^{-7}\text{ cm}} = 12739 \text{ cm}^{-1}$$
$$\tilde{\nu}_{Stokes} = 12739 - 3013 = 9726 \text{ cm}^{-1} \implies \lambda_S = \frac{1}{9726} = \textbf{1028 nm}$$

---

### Q17 — Kerr-Lens Mode Locking (KLM) Description
*(2024 Q3 [6 marks])*

**Question:** The Ti:Sapphire laser uses Kerr-lens mode-locking to generate ultrashort pulses. Describe this phenomenon and explain how it is used to create pulses.

**Model answer (6 marks — aim for 6 distinct points):**

1. **Kerr effect:** The refractive index of the gain crystal is intensity-dependent: n = n₀ + n₂I, where n₂ is the nonlinear refractive index.

2. **Self-focusing:** A Gaussian beam has highest intensity at its centre. The intensity-dependent refractive index is therefore highest at the beam centre → acts as a positive lens. High-intensity pulses self-focus more tightly than low-intensity CW radiation.

3. **Aperture selection:** A hard aperture (or the gain medium geometry acting as a soft aperture) is placed in the cavity such that the tightly-focused pulsed beam passes through it more efficiently than the diffuse CW beam.

4. **Positive feedback:** Any fluctuation that creates a short intense pulse → stronger Kerr lensing → tighter focus → better coupling through aperture → higher gain → pulse amplified at the expense of CW modes.

5. **Not self-starting:** KLM requires an initial perturbation (mirror tap) to launch pulsing. Unlike SESAM, there is no slow saturable absorber to initiate mode-locking spontaneously.

6. **Result:** Near-instantaneous (electronic) Kerr effect allows sub-100 fs pulses, limited by the gain bandwidth of Ti:Sapphire (~100 nm centred at 800 nm) rather than by any absorber recovery time.

---

### Q18 — Gouy Phase: FWM in Bulk vs THG at Interfaces
*(2025 Q2 [2 marks]; 2024 Q2 [2 marks])*

**Question:** The Gouy phase shift is an additional phase change of π radians acquired by a focused Gaussian beam passing through its focal point. Demonstrate why this allows FWM to propagate in the forward direction from bulk material whereas forward THG is only generated at interfaces.

**Model answer:**

The driving nonlinear polarization P⁽ⁿ⁾ ∝ Eⁿ accumulates n times the Gouy phase of the fundamental. The generated harmonic field accumulates its own π Gouy phase.

**For THG (3ω from ω):**
- P⁽³⁾ ∝ E³ accumulates 3π of Gouy phase
- Generated 3ω field accumulates π
- Net mismatch = 3π − π = 2π → effective ΔkL = 2π for bulk → sinc²(ΔkL/2) = sinc²(π) = 0
- THG is phase-matched only when L < λ/3 → interfaces and sub-λ objects only

**For FWM/CARS (ω_p + ω_p − ω_s → ω_as):**
- P⁽³⁾ ∝ E_p² × E_s* accumulates 2π − π = π of Gouy phase (conjugate Stokes contributes −π)
- Generated anti-Stokes at ω_as accumulates +π
- Net mismatch = π − π = 0 → FWM is Gouy-phase-matched forward in bulk

Therefore FWM/CARS generates efficiently from bulk material in the forward direction, while THG requires interfaces.

---

### Q19 — CARS Pulse Parameters and Bandwidth
*(2025 Q4 [2+2+2 marks])*

**Question:** A CARS Stokes laser produces 1 ps pulses at 1064 nm, 80 MHz, 10 mW. Calculate (a) pulse energy, (b) peak power, (c) pulse bandwidth in microns.

**Solution:**

**(a)** $E_{pulse} = P/f = 10\times10^{-3}/80\times10^6 = \textbf{0.125 nJ}$

**(b)** $P_{peak} = E/\tau = 1.25\times10^{-10}/1\times10^{-12} = \textbf{125 W}$

**(c)** Bandwidth:
$$\Delta\nu = \frac{0.441}{1\times10^{-12}} = 4.41\times10^{11} \text{ Hz}$$
$$\Delta\lambda = \frac{\lambda^2}{c}\Delta\nu = \frac{(1064\times10^{-9})^2}{3\times10^8} \times 4.41\times10^{11} = \textbf{1.66 nm} = 1.66\times10^{-3}\text{ µm}$$

In wavenumbers: **14.7 cm⁻¹** — matches the Raman linewidth of ~10–20 cm⁻¹, confirming that ps pulses are optimal for CARS.

---

### Q20 — Rayleigh Scattering Ratio Between Two Wavelengths
*(2025 Q2 [2 marks])*

**Question:** Calculate the relative change in Rayleigh scattering between 532 nm and 1064 nm excitation.

**Solution:**

Rayleigh scattering intensity: $I_{scatter} \propto \frac{1}{\lambda^4}$

$$\frac{I_{532}}{I_{1064}} = \left(\frac{\lambda_{1064}}{\lambda_{532}}\right)^4 = \left(\frac{1064}{532}\right)^4 = 2^4 = \textbf{16}$$

Scattering at 532 nm is **16× stronger** than at 1064 nm. 2PEF (using ~800–1064 nm) therefore penetrates ~16× deeper than single-photon confocal (using ~400–532 nm) in scattering tissue.
