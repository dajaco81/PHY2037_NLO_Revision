# Vital Exam Concepts

All red-box items and explicit exam hints from lectures, organised by topic. If a concept is on this list, it WILL appear in the exam in some form.

---

## From Prerequisite Physics (L02)

### RED BOX: Intensity from electric field
$$I = \frac{1}{2}c\varepsilon_0 E^2$$
*You need to know this to convert atomic field strength into required laser intensity.*

### RED BOX: FWHM of a Gaussian
$$\text{FWHM} = 2\sqrt{2\ln 2}\cdot\sigma \approx 2.355\sigma$$
*Can be asked as: "derive the relationship between FWHM and standard deviation".*

### RED BOX: Energy-time uncertainty principle
$$\Delta E \cdot \Delta t \geq \frac{\hbar}{2}$$
*Links to pulse bandwidth: short pulses → broad bandwidth.*

### CRITICAL: Bandwidth conversion
$$|\Delta\lambda| = \frac{\lambda^2}{c}|\Delta\nu|$$
*Cannot linearly convert Δf to Δλ. This derivation (differentiating f = c/λ) is tested almost every year. Get the factor of λ² right.*

---

## From Contrast Mechanisms (L03–L04)

### RED BOX: Jablonski diagram
Draw with:
- Thick horizontal lines = electronic energy levels (S₀, S₁)
- Thin lines = vibrational sublevels
- **Solid upward arrows** = photon absorption (optical)
- **Solid downward arrows** = photon emission (fluorescence)
- **Wavy arrows** = non-radiative vibrational relaxation (heat)

*The lecturer: "Make sure you can draw these — they always come up"*

### RED BOX: Beer-Lambert law
$$A = \log\left(\frac{I_0}{I_T}\right) = \varepsilon c l$$
*Know what each term means and why you need a known thickness for quantitative imaging.*

### RED BOX: Rayleigh criterion → NA form (derivation)
Derive: d_min = 0.61λ/NA from θ_min = 1.22λ/D

Key steps: θ = d/f; D = 2f·sinα; substitute and simplify.

### Know: Rayleigh scattering
$$I_{scatter} \propto \frac{1}{\lambda^4}$$
*Doubling wavelength reduces scattering by factor 2⁴ = 16. The sky is blue for this reason.*

---

## From Lorentz Oscillator (L05)

### RED BOX: Lorentz oscillator derivation → χ(ω)
Starting point: mṙ̈ + mγṙ + mω₀²r = qE₀e^{-iωt}

Method: assume r = r₀e^{-iωt}; substitute; solve for r₀; get μ = qr₀; get α; multiply by N/ε₀ to get χ.

Result: χ⁽¹⁾(ω) = [Nq²/(mε₀)] / [(ω₀²−ω²)−iγω]

*"This is the kind of derivation I'll ask you to do."*

---

## From Vibrational Spectroscopy (L07)

### RED BOX: Selection rules (BOTH, not just one)

| Technique | Selection rule |
|-----------|---------------|
| IR absorption | Change in **dipole moment** (dμ/dQ ≠ 0) |
| Raman scattering | Change in **polarizability** (dα/dQ ≠ 0) |

*These are complementary and both will be tested. Know which is which.*

### Know: Raman sideband derivation
μ = αE; α oscillates as bond vibrates; product gives sidebands at ω_L ± ω_vib.

### Know: Vibrational frequency formula
ν_vib = (1/2π)√(k/μ_r); μ_r = m₁m₂/(m₁+m₂)

---

## From Nonlinear Susceptibilities (L08–L09)

### RED BOX: χ estimates
At E = E_at: χ⁽¹⁾ ≈ χ⁽²⁾E_at → χ⁽²⁾ ≈ 1/E_at ≈ 2×10⁻¹² m/V
Similarly: χ⁽³⁾ ≈ 1/E_at² ≈ 4×10⁻²⁴ m²/V²

### RED BOX: Units of χ
χ⁽¹⁾: dimensionless; χ⁽²⁾: m/V; χ⁽³⁾: m²/V²

### RED BOX: Centrosymmetry → χ⁽²⁾ = 0
Argument: when E → −E, P⁽²⁾ = ε₀χ⁽²⁾E² stays positive (doesn't reverse). Physical displacement must reverse. Contradiction → χ⁽²⁾ = 0.

### RED BOX: SHG perturbation derivation
Full derivation using perturbation technique. For exam: SHG, SFG, or DFG — same method.

---

## From Wave Equation and Phase Matching (L10–L11)

### RED BOX: Nonlinear wave equation
∇²E − (n²/c²)∂²E/∂t² = (1/ε₀c²)∂²P_NL/∂t²

Derivation: Maxwell's equations → take curl → use vector identity → substitute D = ε₀n²E + P_NL.

### RED BOX: Coupled amplitude equation (SFG)
dA₃/dz = (iω₃d_eff/n₃c)A₁A₂e^{iΔkz}

Derivation: write fields as A_j(z)e^{i(k_jz−ω_jt)}; substitute into wave eq; SVEA (drop ∂²A/∂z²); cancel k²/n² terms.

**Key step:** A is a function of z — use product rule when differentiating E.

### RED BOX: Signal intensity
I₃ ∝ L² sinc²(ΔkL/2)

Know: maximum at Δk=0; first zero at ΔkL/2 = π.

### RED BOX: Gouy phase shift and implications
- Gouy phase = π total through a focused beam
- SHG: L < λ/2 (achievable) → works in microscope
- THG: L < λ/3 (very hard) → only interfaces

---

## From Laser Pulses (L12, L14)

### RED BOX: Pulse parameter equations
E_pulse = P_av/f_rep; P_peak = E_pulse/τ_p; I_peak = P_peak/A

*"You need to memorise these — they're not given."*

### RED BOX: Time-bandwidth product
Δν·Δt = 2ln2/π ≈ 0.441 (Gaussian pulses)

Full derivation from Fourier transform of Gaussian — the Fourier transform itself is given.

### CRITICAL: Bandwidth conversion (appears every year)
Δλ = (λ²/c)Δν — must differentiate f = c/λ; do NOT substitute directly.

---

## From NLO Microscopy (L14–L15)

### RED BOX: Three advantages of NLO over conventional
1. No pinhole (signal only from focal volume; scales as Iⁿ)
2. Deeper penetration (2× wavelength → 16× less Rayleigh scattering)
3. Resolution partially recovered (FWHM_nP = FWHM_1P/√n)

### RED BOX: Resolution squeeze derivation
2PEF signal ∝ I² = exp(−2r²/σ²) = exp(−r²/(σ/√2)²) → effective σ = σ/√2 → FWHM/√2

### RED BOX: Parametric vs. non-parametric

| Type | Definition | Phase matching? | Examples |
|------|-----------|----------------|---------|
| Parametric | No net energy transfer to material; quantum state unchanged | Required (coherent) | SHG, SFG, THG, CARS |
| Non-parametric | Energy deposited; quantum state changes | Not required | Fluorescence, SRS, IR absorption |

---

## From CARS/SRS (L16)

### RED BOX: CARS wavelength calculations

Stokes: λ_S = 1/(1/λ_P − ν̃_vib) [λ in cm, ν̃ in cm⁻¹]

Anti-Stokes: λ_AS = 1/(1/λ_P + ν̃_vib) [λ in cm]

Sanity check: λ_S > λ_P; λ_AS < λ_P

### Know: Why ps pulses for CARS/SRS
Raman linewidth ~10–20 cm⁻¹ → requires Δν < linewidth → Δt > 1/(Δν) ~ ps.
Using 100 fs pulses → ~330 cm⁻¹ bandwidth → excites many Raman peaks simultaneously → loses chemical selectivity.

---

## From Laser Sources (L17)

### Know: Mode locking
- SESAM: semiconductor saturable absorber → suitable for ps pulses
- KLM: Kerr lens (n = n₀ + n₂I) → suitable for fs pulses
- Difference: SESAM relaxation time ~ps limits pulse width; KLM is near-instantaneous

### RED BOX: OPO wavelength equation
1/λ_P = 1/λ_S + 1/λ_i

---

## From Applications (L18)

### RED BOX: Forward vs. backward CARS
Forward: bulk material → phase matched → strong signal
Backward (EPI): Δk very large → only sub-λ objects → nanoparticle detection

*"Phase matching derivation was worthwhile. Now you understand why backwards CARS is selective."*

### Know: Deuterium labelling
D replaces H → C–D stretch shifts to ~2100 cm⁻¹ (silent region). Minimal chemical perturbation. Unique Raman signature.

---

## Likely Exam Question Types

1. **Derivation:** χ⁽¹⁾ from Lorentz model (D01); TBP (D06); wave equation (D07); coupled amplitude (D08); resolution squeeze (D10)
2. **Derivation:** SHG susceptibility using perturbation theory (D02)
3. **Derivation:** Rayleigh criterion → NA form (D04)
4. **Calculation:** Pulse energy/power/intensity from P_av, f_rep, τ_p, A
5. **Calculation:** CARS wavelengths from pump λ and Raman shift ν̃
6. **Calculation:** Bandwidth from TBP; convert to Δλ
7. **Explanation:** Why χ⁽²⁾ = 0 for centrosymmetric materials
8. **Explanation:** Three advantages of 2PEF over 1PEF
9. **Draw:** Jablonski diagram; confocal microscopy setup; mode locking loss curve
10. **Compare:** IR vs Raman; CARS vs SRS; SESAM vs KLM
