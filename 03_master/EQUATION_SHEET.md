# PHY2037 Equation Sheet

All examinable equations. **Bold** = in a red box (must memorise). Others are derivable or given on exam front sheet.

---

## 1. Electromagnetism Fundamentals

**1.1** Electric force on a charge:  
$$\mathbf{F} = q\mathbf{E}$$

**1.2** Linear polarisation (dipole moment per unit volume):  
$$\mathbf{P} = \varepsilon_0 \chi^{(1)} \mathbf{E}$$

**1.3** Displacement field:  
$$\mathbf{D} = \varepsilon_0 \mathbf{E} + \mathbf{P}$$

**1.4 [RED BOX]** Intensity from electric field amplitude:  
$$I = \frac{1}{2}c\varepsilon_0 |E|^2$$

**1.5** Linear wave equation:  
$$\nabla^2\mathbf{E} = \frac{n^2}{c^2}\frac{\partial^2\mathbf{E}}{\partial t^2}$$

**1.6** Wave vector:  
$$k = \frac{n\omega}{c}$$

---

## 2. Harmonic Oscillator / Lorentz Model

**2.1** Equation of motion for bound charge:  
$$m\ddot{r} + m\gamma\dot{r} + m\omega_0^2 r = qE_0 e^{-i\omega t}$$

**2.2** Resonant frequency:  
$$\omega_0 = \sqrt{k/m}$$

**2.3 [RED BOX]** Linear electric susceptibility (result of Lorentz model):  
$$\chi^{(1)}(\omega) = \frac{Nq^2}{m\varepsilon_0} \cdot \frac{1}{(\omega_0^2 - \omega^2) - i\gamma\omega}$$

**2.4** Detuning function: D(ω) = ω₀² − ω² − iγω

---

## 3. Atomic / Quantum Mechanics

**3.1** Bohr radius:  
$$a_0 = \frac{4\pi\varepsilon_0\hbar^2}{me^2} \approx 0.53 \text{ Å}$$

**3.2 [RED BOX]** Atomic field strength (threshold for NLO):  
$$E_{at} = \frac{e}{4\pi\varepsilon_0 a_0^2} \approx 5\times10^{11} \text{ V m}^{-1}$$

**3.3** Hydrogen atom energy levels:  
$$E_n = -\frac{13.6 \text{ eV}}{n^2}$$

**3.4** Infinite square well energy levels:  
$$E_n = \frac{n^2h^2}{8mL^2}$$

**3.5 [RED BOX]** Energy-time uncertainty principle:  
$$\Delta E \cdot \Delta t \geq \frac{\hbar}{2}$$

---

## 4. Gaussian Functions and Fourier Transforms

**4.1 [RED BOX]** FWHM of a Gaussian (amplitude):  
$$\text{FWHM}_{amplitude} = 2\sqrt{2\ln 2}\cdot\sigma \approx 2.355\sigma$$

**4.2** FWHM of intensity Gaussian (I = E²):  
$$\text{FWHM}_{intensity} = \sqrt{2}\cdot\text{FWHM}_{amplitude}/\sqrt{2} = 2\sqrt{\ln 2}\cdot\sigma$$

**4.3** Fourier transform of Gaussian (given on exam):  
$$\mathcal{F}\{e^{-t^2/2\sigma^2}\} \propto e^{-\omega^2\sigma^2/2}$$

**4.4 [RED BOX]** Bandwidth conversion:  
$$|\Delta\lambda| = \frac{\lambda^2}{c}|\Delta\nu|$$

---

## 5. Vibrational Spectroscopy

**5.1** Vibrational frequency of a diatomic molecule:  
$$\nu_{vib} = \frac{1}{2\pi}\sqrt{\frac{k}{\mu_r}}$$

**5.2** Reduced mass:  
$$\mu_r = \frac{m_1 m_2}{m_1 + m_2}$$

**5.3** Wavenumber:  
$$\tilde{\nu} = \frac{1}{\lambda} = \frac{\nu}{c} \quad [\text{cm}^{-1}]$$

**5.4 [RED BOX]** IR selection rule: Absorption requires change in dipole moment (dμ/dQ ≠ 0)

**5.5 [RED BOX]** Raman selection rule: Scattering requires change in polarizability (dα/dQ ≠ 0)

**5.6** Raman Stokes shift:  
$$\tilde{\nu}_{Stokes} = \frac{1}{\lambda_P} - \frac{1}{\lambda_S} \quad [\text{both in cm}]$$

---

## 6. Nonlinear Susceptibilities

**6.1 [RED BOX]** Nonlinear power series:  
$$\mathbf{P} = \varepsilon_0\left[\chi^{(1)}\mathbf{E} + \chi^{(2)}\mathbf{E}^2 + \chi^{(3)}\mathbf{E}^3 + \cdots\right]$$

**6.2 [RED BOX]** χ⁽²⁾ estimate:  
$$\chi^{(2)} \approx \frac{\chi^{(1)}}{E_{at}} \approx 2\times10^{-12} \text{ m V}^{-1}$$

**6.3 [RED BOX]** χ⁽³⁾ estimate:  
$$\chi^{(3)} \approx \frac{\chi^{(1)}}{E_{at}^2} \approx 4\times10^{-24} \text{ m}^2\text{V}^{-2}$$

**6.4 [RED BOX]** Units of χ: χ⁽¹⁾ dimensionless; χ⁽²⁾ in m/V; χ⁽³⁾ in m²/V²

**6.5 [RED BOX]** Centrosymmetry → χ⁽²⁾ = 0

---

## 7. Wave Equation and Phase Matching

**7.1 [RED BOX]** Nonlinear wave equation:  
$$\nabla^2\mathbf{E} - \frac{n^2}{c^2}\frac{\partial^2\mathbf{E}}{\partial t^2} = \frac{1}{\varepsilon_0 c^2}\frac{\partial^2\mathbf{P}_{NL}}{\partial t^2}$$

**7.2 [RED BOX]** Phase matching condition:  
$$\mathbf{k}_3 = \mathbf{k}_1 + \mathbf{k}_2 \quad (\Delta k = 0)$$

**7.3 [RED BOX]** Coupled amplitude equation (SFG):  
$$\frac{dA_3}{dz} = \frac{i\omega_3 d_{eff}}{n_3 c} A_1 A_2 e^{i\Delta k z}$$

**7.4 [RED BOX]** Signal intensity vs. phase mismatch:  
$$I_3 \propto L^2 \,\text{sinc}^2\!\left(\frac{\Delta k L}{2}\right)$$

**7.5** Coherence length (first zero):  
$$L_c = \frac{\pi}{\Delta k}$$

**7.6** Quasi-phase matching period:  
$$\Lambda = \frac{2\pi}{\Delta k}$$

---

## 8. Laser Pulses

**8.1 [RED BOX]** Pulse energy:  
$$E_{pulse} = \frac{P_{av}}{f_{rep}}$$

**8.2 [RED BOX]** Peak power:  
$$P_{peak} = \frac{E_{pulse}}{\tau_p}$$

**8.3 [RED BOX]** Peak intensity:  
$$I_{peak} = \frac{P_{peak}}{A}$$

**8.4 [RED BOX]** Time-bandwidth product (Gaussian pulses):  
$$\Delta\nu \cdot \Delta t = \frac{2\ln 2}{\pi} \approx 0.441$$

---

## 9. Microscopy and NLO Imaging

**9.1** Numerical aperture:  
$$\text{NA} = n\sin\alpha$$

**9.2 [RED BOX]** Abbe diffraction limit:  
$$d = \frac{\lambda}{2\,\text{NA}}$$

**9.3** Rayleigh criterion (angular):  
$$\theta_{min} = \frac{1.22\lambda}{D}$$

**9.4 [RED BOX]** Rayleigh criterion → NA form (must derive):  
$$d_{min} = \frac{0.61\lambda}{\text{NA}}$$

**9.5** Rayleigh scattering:  
$$I_{scatter} \propto \frac{1}{\lambda^4}$$

**9.6 [RED BOX]** Nonlinear resolution squeeze:  
$$\text{FWHM}_{nP} = \frac{\text{FWHM}_{1P}}{\sqrt{n}}$$

---

## 10. CARS and SRS

**10.1 [RED BOX]** CARS Stokes wavelength:  
$$\frac{1}{\lambda_S} = \frac{1}{\lambda_P} - \tilde{\nu}_{vib} \quad [\lambda\text{ in cm}]$$

**10.2 [RED BOX]** CARS anti-Stokes wavelength:  
$$\frac{1}{\lambda_{AS}} = \frac{1}{\lambda_P} + \tilde{\nu}_{vib} \quad [\lambda\text{ in cm}]$$

**10.3** CARS four-wave mixing: ω_AS = 2ω_P − ω_S

---

## 11. Laser Sources

**11.1** Cavity mode spacing:  
$$\Delta\nu = \frac{c}{2L}$$

**11.2** Kerr effect (intensity-dependent refractive index):  
$$n = n_0 + n_2 I$$

**11.3 [RED BOX]** OPO energy conservation:  
$$\frac{1}{\lambda_P} = \frac{1}{\lambda_S} + \frac{1}{\lambda_i}$$

---

## Equations Given on Exam Front Sheet

The following will be provided (do not need to memorise):
- Fourier transform of a Gaussian
- Standard integrals for sinc² phase matching derivation
- The specific Bessel function form of the Airy disk (if needed)
