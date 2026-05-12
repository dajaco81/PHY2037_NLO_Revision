# Derivation Practice

Derivation exercises stripped of working. Attempt each one from scratch, then check against the full worked version in `03_master/DERIVATION_BANK.md`.

---

## P01 — Linear Susceptibility from Lorentz Model

**Task:** Derive an expression for χ⁽¹⁾(ω), the linear electric susceptibility of a dielectric material.

**Starting point:**
$$m\ddot{r} + m\gamma\dot{r} + m\omega_0^2 r = qE_0 e^{-i\omega t}$$

**Hints (cover these until needed):**
1. Assume r = r₀e^{-iωt}
2. Substitute; differentiate; collect r₀ terms
3. Get r₀; then μ = qr₀; then α = μ/E₀; then χ⁽¹⁾ = Nα/ε₀

**Expected result:**
$$\chi^{(1)}(\omega) = \frac{Nq^2}{m\varepsilon_0[({\omega_0^2 - \omega^2}) - {i\gamma\omega}]}$$

---

## P02 — SHG Susceptibility via Perturbation Theory

**Task:** Using the perturbation technique, derive χ⁽²⁾(2ω;ω,ω) for second harmonic generation in a non-centrosymmetric material.

**Starting point:**
$$m\ddot{r} + m\gamma\dot{r} + m\omega_0^2 r + mar^2 = qE_0 e^{-i\omega t}$$

**Hints:**
1. Replace E → λE; r = λr₁ + λ²r₂ + ...
2. Show first-order gives the Lorentz result
3. Show second-order is driven by −(a/m)r₁²
4. Seek r₂ ∝ e^{-2iωt}; solve for amplitude
5. Get χ⁽²⁾ via dipole → polarizability → susceptibility

**Expected result (schematic):**
$$\chi^{(2)}(2\omega;\omega,\omega) \propto \frac{-aq^3/m^2\varepsilon_0}{D(\omega)^2 D(2\omega)}$$
where D(ω) = ω₀² − ω² − iγω

---

## P03 — Why χ⁽²⁾ = 0 for Centrosymmetric Materials

**Task:** Using the perturbation expansion with the symmetric potential (r³ term), prove mathematically that χ⁽²⁾ = 0.

**Starting point:**
$$m\ddot{r} + m\gamma\dot{r} + m\omega_0^2 r + mbr^3 = qE_0 e^{-i\omega t}$$

**Hint:** Expand r³ = (λr₁ + λ²r₂ + …)³ and show there are no λ² terms to drive the second-order equation.

---

## P04 — FWHM of a Gaussian

**Task:** Derive FWHM = 2√(2ln2)·σ for an amplitude Gaussian f(x) = f₀exp(−x²/2σ²).

**Hint:** Set f(x₁/₂) = f₀/2; take logarithm; solve for x₁/₂; multiply by 2.

---

## P05 — Rayleigh Criterion → NA Form

**Task:** Convert θ_min = 1.22λ/D (angular Rayleigh criterion) into d_min = 0.61λ/NA (distance resolution for a microscope).

**Hints:**
1. In a microscope: d = f·θ (small angle)
2. Half-angle at lens: sin(α) ≈ D/(2f)
3. Substitute; simplify using NA = n·sinα

---

## P06 — Time-Bandwidth Product

**Task:** Derive Δν·Δt = 2ln2/π ≈ 0.441 for transform-limited Gaussian pulses.

**Starting point:** E(t) = E₀exp(−t²/2σ_t²); Fourier transform (given): Ẽ(ν) ∝ exp(−2π²ν²σ_t²)

**Hint:** Convert amplitude FTs to intensity; find FWHM_t and FWHM_ν separately; multiply.

---

## P07 — Nonlinear Wave Equation

**Task:** Derive the nonlinear wave equation starting from Maxwell's equations, showing that P_NL acts as a source term.

**Starting point:** Maxwell's equations in matter (∇×H = ∂D/∂t; ∇×E = −∂B/∂t)

**Hints:**
1. Take curl of one Maxwell equation
2. Use vector identity ∇×(∇×E) = ∇(∇·E) − ∇²E
3. Set ∇·E ≈ 0; substitute D = ε₀n²E + P_NL
4. Rearrange to move P_NL to RHS

**Expected result:**
$$\nabla^2\mathbf{E} - \frac{n^2}{c^2}\frac{\partial^2\mathbf{E}}{\partial t^2} = \frac{1}{\varepsilon_0 c^2}\frac{\partial^2\mathbf{P}_{NL}}{\partial t^2}$$

---

## P08 — Coupled Amplitude Equation

**Task:** Derive dA₃/dz = (iω₃d_eff/n₃c) A₁A₂e^{iΔkz} for sum frequency generation ω₃ = ω₁+ω₂.

**Starting point:** Nonlinear wave equation; write E_j = A_j(z)exp[i(k_jz−ω_jt)] + c.c.

**Critical hint:** When differentiating E₃ = A₃(z)exp[i(k₃z−ω₃t)] twice with respect to z:
$$\frac{\partial^2 E_3}{\partial z^2} = \left(\frac{\partial^2 A_3}{\partial z^2} + 2ik_3\frac{\partial A_3}{\partial z} - k_3^2 A_3\right)e^{i(k_3z-\omega_3t)}$$
Then apply SVEA (drop ∂²A/∂z²) and note k₃² cancels with n₃²ω₃²/c².

---

## P09 — Signal Intensity sinc² Form

**Task:** Integrate the coupled amplitude equation (undepleted pump: A₁, A₂ constant) from 0 to L to show I₃ ∝ L² sinc²(ΔkL/2).

**Hint:** ∫₀ᴸ e^{iΔkz}dz = (e^{iΔkL}−1)/(iΔk); take |A₃|²; use |e^{iθ}−1|² = 4sin²(θ/2).

---

## P10 — Nonlinear Resolution Squeeze

**Task:** Show that for two-photon excitation, the effective PSF FWHM is reduced by a factor of √2 compared to a single-photon PSF of the same shape.

**Starting point:** I_1P(r) ∝ exp(−r²/σ²); I_2PEF ∝ [I_1P]²

**Hint:** Square the Gaussian; identify the new effective σ; convert to FWHM.

---

## Checklist: Must be able to derive without notes

- [ ] P01: Lorentz χ(ω)
- [ ] P02: SHG χ⁽²⁾ via perturbation
- [ ] P03: χ⁽²⁾=0 for centrosymmetric
- [ ] P04: Gaussian FWHM
- [ ] P05: Rayleigh criterion → NA
- [ ] P06: Time-bandwidth product
- [ ] P07: Nonlinear wave equation
- [ ] P08: Coupled amplitude equation
- [ ] P09: sinc² signal intensity
- [ ] P10: Nonlinear resolution squeeze
