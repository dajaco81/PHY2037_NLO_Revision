# PHY2037 Derivation Bank

All examinable derivations from the lecture course. Each entry includes: what is being derived, the starting point, the method, and the key steps.

---

## D01 — Linear Susceptibility χ⁽¹⁾(ω) from the Lorentz Oscillator Model

**[RED BOX — highly likely exam question]**

**What:** Derive χ⁽¹⁾(ω) — show how the susceptibility of a material depends on the frequency of the applied EM field.

**Starting point:**
$$m\ddot{r} + m\gamma\dot{r} + m\omega_0^2 r = qE_0 e^{-i\omega t}$$

**Method:** Assume solution r = r₀e^{-iωt} (sinusoidal at driving frequency)

**Steps:**

1. **Differentiate:** ṙ = −iωr₀e^{-iωt}; r̈ = −ω²r₀e^{-iωt}

2. **Substitute:**
$$m(-\omega^2) r_0 + m\gamma(-i\omega) r_0 + m\omega_0^2 r_0 = qE_0$$
$$r_0[(m\omega_0^2 - m\omega^2) - im\gamma\omega] = qE_0$$

3. **Solve for r₀:**
$$r_0 = \frac{qE_0/m}{(\omega_0^2 - \omega^2) - i\gamma\omega} \equiv \frac{qE_0/m}{D(\omega)}$$

4. **Dipole moment:** μ = qr₀

5. **Polarizability:** α = μ/E₀ = q²/(mD(ω))

6. **Polarisation per unit volume** (N atoms):
$$P = N\alpha\varepsilon_0 E = \varepsilon_0\chi^{(1)}E$$

7. **Result:**
$$\boxed{\chi^{(1)}(\omega) = \frac{Nq^2}{m\varepsilon_0} \cdot \frac{1}{(\omega_0^2 - \omega^2) - i\gamma\omega}}$$

---

## D02 — Second-Order Susceptibility χ⁽²⁾ for SHG (Perturbation Theory)

**[RED BOX — very likely exam question]**

**What:** Derive χ⁽²⁾(2ω;ω,ω) using perturbation theory on the anharmonic oscillator.

**Starting point (non-centrosymmetric):**
$$m\ddot{r} + m\gamma\dot{r} + m\omega_0^2 r + mar^2 = qE_0 e^{-i\omega t}$$

**Method:** Perturbation expansion r = λr₁ + λ²r₂ + …; collect terms at each power of λ.

**Steps:**

1. **Replace E → λE; expand r in powers of λ**

2. **First order (λ¹ terms):**
$$m\ddot{r}_1 + m\gamma\dot{r}_1 + m\omega_0^2 r_1 = qE_0e^{-i\omega t}$$
→ Same as linear Lorentz → $r_1^{(\omega)} = \frac{qE_0/m}{D(\omega)}e^{-i\omega t}$

3. **Second order (λ² terms):** The r² term contributes a driving force −m·a·r₁²:
$$m\ddot{r}_2 + m\gamma\dot{r}_2 + m\omega_0^2 r_2 = -ma \cdot r_1^2$$

4. **Compute r₁² and pick out the e^{-2iωt} component:**
$$r_1^2 = (r_1^{(\omega)})^2 e^{-2i\omega t} + \text{other terms}$$

5. **Seek solution** r₂ = r₂⁽²ω⁾e^{-2iωt}; substitute:
$$D(2\omega) \cdot r_2^{(2\omega)} = -\frac{a}{m}\left(\frac{qE_0/m}{D(\omega)}\right)^2$$

6. **Solve:**
$$r_2^{(2\omega)} = \frac{-a q^2 E_0^2/m^3}{D(\omega)^2 D(2\omega)}$$

7. **Get χ⁽²⁾:**
$$\chi^{(2)}(2\omega;\omega,\omega) = \frac{N \cdot q^3/m^2 \cdot (-a)}{\varepsilon_0 \cdot D(\omega)^2 \cdot D(2\omega)}$$

**For other second-order processes (SFG, DFG):** same method, seek solution at ω₁±ω₂ instead of 2ω.

---

## D03 — Proof that χ⁽²⁾ = 0 for Centrosymmetric Materials

**[RED BOX]**

**Method 1 (physical argument):**
P⁽²⁾ = ε₀χ⁽²⁾E². When E → −E: E² → (−E)² = +E². So P⁽²⁾ stays positive — doesn't change sign. But P is a physical displacement vector and should reverse when E reverses in a centrosymmetric material. Contradiction → χ⁽²⁾ = 0.

**Method 2 (from perturbation theory):**
For centrosymmetric material, the nonlinear term is r³ (symmetric). Expand r³ = (λr₁ + λ²r₂ + …)³. The lowest power contribution is λ³·r₁³ (the r³ term contributes nothing at order λ² since (λr₁)³ = λ³r₁³). So the λ² equation of motion has zero on the right-hand side → no solution → χ⁽²⁾ = 0. ∎

---

## D04 — Rayleigh Criterion: Converting from Angle to Distance via NA

**[RED BOX — derivation]**

**What:** Convert the angular Rayleigh criterion θ_min = 1.22λ/D to a distance resolution d_min using NA.

**Starting point:** θ_min = 1.22λ/D (angular criterion from diffraction theory)

**Steps:**

1. In a microscope with lens focal length f and lens diameter D:
$$\theta = \frac{d_{min}}{f}$$

2. The half-angle α at the lens satisfies: tan(α) ≈ sin(α) = D/(2f) (small angle)
→ D = 2f·sin(α)

3. Substitute into Rayleigh criterion:
$$d_{min} = 1.22\frac{\lambda f}{D} = 1.22\frac{\lambda f}{2f\sin\alpha} = \frac{1.22\lambda}{2\sin\alpha}$$

4. For a lens in medium of refractive index n (general case): sin(α) → NA/n, so sinα = NA/n:
$$d_{min} = \frac{0.61\lambda}{NA}$$

---

## D05 — FWHM of a Gaussian

**[RED BOX]**

**What:** Derive the relationship between FWHM and standard deviation σ for a Gaussian function.

**Starting point:** f(x) = f₀ exp(−x²/2σ²)

**Steps:**

1. At FWHM: f(x₁/₂) = f₀/2
$$\frac{1}{2} = e^{-x_{1/2}^2/2\sigma^2}$$

2. Take ln of both sides:
$$\ln\frac{1}{2} = -\frac{x_{1/2}^2}{2\sigma^2} \implies x_{1/2}^2 = 2\sigma^2\ln 2$$
$$x_{1/2} = \sigma\sqrt{2\ln 2}$$

3. Full width = 2x₁/₂:
$$\boxed{\text{FWHM} = 2\sigma\sqrt{2\ln 2} \approx 2.355\sigma}$$

**For intensity Gaussian** I(t) = I₀ exp(−t²/σ_t²) (note: σ_t not 2σ²):
At half-max: ½ = exp(−t²/σ_t²) → t₁/₂ = σ_t√(ln2)
FWHM_intensity = 2σ_t√(ln2) = FWHM_amplitude/√2 (narrower by √2 due to squaring)

---

## D06 — Time-Bandwidth Product for Gaussian Pulses

**[RED BOX]**

**What:** Derive Δν·Δt = 2ln2/π ≈ 0.441 for transform-limited Gaussian pulses.

**Starting point:** E(t) = E₀ exp(−t²/2σ_t²); Fourier transform (given): Ẽ(ν) ∝ exp(−2π²ν²σ_t²)

**Steps:**

1. **Intensity in time:** I(t) = |E|² ∝ exp(−t²/σ_t²)
   - At FWHM: ½ = exp(−t²/σ_t²) → t₁/₂ = σ_t√(ln2)
   - Δt = FWHM_t = 2σ_t√(ln2)

2. **Intensity in frequency:** I(ν) ∝ exp(−4π²ν²σ_t²)
   - At FWHM: ½ = exp(−4π²ν²σ_t²) → ν₁/₂ = √(ln2)/(2πσ_t)
   - Δν = FWHM_ν = √(ln2)/(πσ_t)

3. **Product:**
$$\Delta\nu \cdot \Delta t = \frac{\sqrt{\ln2}}{\pi\sigma_t} \times 2\sigma_t\sqrt{\ln 2} = \frac{2\ln 2}{\pi} \approx 0.441$$

---

## D07 — Nonlinear Wave Equation

**[RED BOX]**

**What:** Derive the nonlinear wave equation from Maxwell's equations.

**Steps:**

1. Start from Maxwell: ∇ × **H** = ∂**D**/∂t (no free currents)

2. Take curl: ∇ × (∇ × **E**) = −μ₀ ∂²**D**/∂t²

3. Use vector identity: ∇ × (∇ × **E**) = ∇(∇·**E**) − ∇²**E**; ∇·**E** ≈ 0 (no free charges)

4. Split **D** = ε₀**E** + **P** = ε₀(1+χ⁽¹⁾)**E** + **P**_NL = ε₀n²**E** + **P**_NL

5. Substitute:
$$-\nabla^2\mathbf{E} = -\mu_0\frac{\partial^2}{\partial t^2}\left[\varepsilon_0 n^2\mathbf{E} + \mathbf{P}_{NL}\right]$$

6. Use μ₀ε₀ = 1/c²:
$$\boxed{\nabla^2\mathbf{E} - \frac{n^2}{c^2}\frac{\partial^2\mathbf{E}}{\partial t^2} = \frac{1}{\varepsilon_0 c^2}\frac{\partial^2\mathbf{P}_{NL}}{\partial t^2}}$$

---

## D08 — Coupled Amplitude Equation for SFG

**[RED BOX]**

**What:** Derive dA₃/dz = (iω₃d_eff/n₃c) A₁A₂e^{iΔkz}

**Starting point:** Nonlinear wave equation; write fields as E_j = A_j(z)exp[i(k_j z − ω_j t)] + c.c.

**Steps:**

1. Compute ∂²E₃/∂z²:
$$\frac{\partial^2 E_3}{\partial z^2} = \left(\frac{\partial^2 A_3}{\partial z^2} + 2ik_3\frac{\partial A_3}{\partial z} - k_3^2 A_3\right)e^{ik_3 z}$$

2. **SVEA:** |∂²A_3/∂z²| ≪ |k₃ ∂A₃/∂z| → drop first term

3. **Left side of wave equation** (∂²E₃/∂z² − n₃²ω₃²/c² E₃):
$$\left(2ik_3\frac{\partial A_3}{\partial z} - k_3^2 A_3 + \frac{n_3^2\omega_3^2}{c^2}A_3\right)e^{i(k_3 z - \omega_3 t)}$$
Since k₃ = n₃ω₃/c: k₃² = n₃²ω₃²/c² → terms cancel:
$$= 2ik_3\frac{\partial A_3}{\partial z}e^{i(k_3 z - \omega_3 t)}$$

4. **Right side** (from P_NL at ω₃ = ω₁ + ω₂):
$$\frac{-\omega_3^2}{\varepsilon_0 c^2} \cdot \varepsilon_0\chi^{(2)}A_1A_2 e^{i(k_1+k_2)z} = \frac{-\omega_3^2 d_{eff}}{c^2} A_1 A_2 e^{i(k_1+k_2)z}$$

5. **Equate and simplify:**
$$2ik_3\frac{dA_3}{dz} = \frac{-\omega_3^2 d_{eff}}{c^2} A_1 A_2 e^{i(k_1+k_2-k_3)z} = \frac{-\omega_3^2 d_{eff}}{c^2} A_1 A_2 e^{-i\Delta k z}$$

Substituting k₃ = n₃ω₃/c:
$$\boxed{\frac{dA_3}{dz} = \frac{i\omega_3 d_{eff}}{n_3 c} A_1 A_2 e^{i\Delta k z}}$$

---

## D09 — Signal Intensity ∝ sinc²(ΔkL/2)

**What:** Integrate the coupled amplitude equation to get the signal intensity.

**Starting point:** dA₃/dz = C A₁A₂ e^{iΔkz} where C = iω₃d_eff/(n₃c) and A₁, A₂ are approximately constant (undepleted pump).

**Steps:**

1. Integrate from 0 to L:
$$A_3(L) = C A_1 A_2 \int_0^L e^{i\Delta k z}dz = C A_1 A_2 \left[\frac{e^{i\Delta kL}-1}{i\Delta k}\right]$$

2. Take modulus squared:
$$|A_3(L)|^2 = |C A_1 A_2|^2 \cdot \frac{|e^{i\Delta kL}-1|^2}{\Delta k^2}$$

3. Use |e^{iθ} − 1|² = 4sin²(θ/2):
$$|A_3|^2 \propto \frac{\sin^2(\Delta kL/2)}{(\Delta k/2)^2} = L^2\,\text{sinc}^2\!\left(\frac{\Delta kL}{2}\right)$$

4. Signal intensity:
$$\boxed{I_3 \propto L^2\,\text{sinc}^2\!\left(\frac{\Delta kL}{2}\right)}$$

---

## D10 — Nonlinear Resolution Squeeze

**What:** Show 2PEF has resolution FWHM/√2 relative to single-photon PSF.

**Starting point:** I(r) ∝ exp(−r²/σ²) (single-photon Gaussian PSF)

**Steps:**

1. **2PEF signal** ∝ I²(r) = exp(−2r²/σ²) = exp(−r²/(σ/√2)²)

2. This is a Gaussian with σ_eff = σ/√2 → FWHM_2P = FWHM_1P/√2

3. **Including the wavelength factor** (2PEF uses 2λ):
   - 1PEF FWHM = 0.61λ/NA (at λ_ex)
   - 2PEF FWHM (without squeeze) = 0.61×(2λ_ex)/NA
   - 2PEF FWHM (with squeeze) = 0.61×(2λ_ex)/(NA×√2) = 0.61√2·λ_ex/NA

**General:** For n-photon: FWHM_nP = (0.61 × n·λ_ex/NA) / √n = 0.61√n·λ_ex/NA
