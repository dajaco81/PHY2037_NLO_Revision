# Notation Standardization

This document defines the canonical symbols used throughout this repository. Inconsistencies in the transcripts are resolved here.

---

## Susceptibility

| Symbol | Meaning | Units | Notes |
|--------|---------|-------|-------|
| χ or χ⁽¹⁾ | Linear electric susceptibility | dimensionless | Scalar for isotropic materials; tensor in general |
| χ⁽²⁾ | Second-order nonlinear susceptibility | m V⁻¹ | Zero for centrosymmetric materials |
| χ⁽³⁾ | Third-order nonlinear susceptibility | m² V⁻² | Non-zero for all materials |
| d_eff | Effective nonlinear coefficient (SFG, SHG) | pm V⁻¹ or m V⁻¹ | Scalar approximation for fixed geometry; related to χ⁽²⁾ |

---

## Fields and Polarisation

| Symbol | Meaning | Units |
|--------|---------|-------|
| **E** | Electric field vector | V m⁻¹ (= N C⁻¹) |
| E₀ | Amplitude of electric field | V m⁻¹ |
| **P** | Electric polarisation (induced dipole moment per unit volume) | C m⁻² |
| **D** | Electric displacement field | C m⁻² |
| I | Intensity (time-averaged power per unit area) | W m⁻² |
| k | Wave vector magnitude | m⁻¹ (also rad m⁻¹) |
| Δk | Phase mismatch | m⁻¹ |

---

## Oscillator Model

| Symbol | Meaning |
|--------|---------|
| ω₀ | Natural (resonant) frequency of oscillator (rad s⁻¹) |
| ω | Driving frequency (rad s⁻¹) |
| γ | Damping coefficient (s⁻¹) |
| r | Displacement of charge from equilibrium (m) |
| D(ω) | Detuning denominator: ω₀² − ω² − iγω |
| a | Asymmetric nonlinear coefficient (non-centrosymmetric term) |
| b | Symmetric nonlinear coefficient (centrosymmetric term) |

---

## Quantum Mechanics / Atoms

| Symbol | Meaning | Value |
|--------|---------|-------|
| a₀ | Bohr radius | 0.529 Å = 5.29×10⁻¹¹ m |
| E_at | Atomic electric field strength | ≈ 5×10¹¹ V m⁻¹ |
| μ | Reduced mass (also sometimes dipole moment; context distinguishes) | kg |
| μ_r | Reduced mass | m₁m₂/(m₁+m₂) |
| μ_dipole | Dipole moment | C·m |

---

## Spectroscopy

| Symbol | Meaning | Units |
|--------|---------|-------|
| ν_vib | Vibrational frequency | Hz |
| ω_vib | Vibrational angular frequency | rad s⁻¹ |
| $\tilde{\nu}$ | Wavenumber | cm⁻¹ |
| k (spring) | Bond spring constant | N m⁻¹ (= kg s⁻²) |
| α | Polarizability (single atom/bond) | C² s² kg⁻¹ m⁻³ (or Å³) |
| Q | Normal coordinate (bond displacement) | Å or m |

---

## Laser Pulses

| Symbol | Meaning | Units |
|--------|---------|-------|
| P_av | Average laser power | W |
| f_rep | Repetition rate | Hz |
| τ_p | Pulse duration (FWHM of intensity) | s |
| E_pulse | Energy per pulse | J |
| P_peak | Peak power | W |
| I_peak | Peak intensity | W m⁻² |
| Δt | Pulse duration (FWHM) | s |
| Δν | Bandwidth (FWHM) | Hz |
| σ_t | Standard deviation of intensity Gaussian (time) | s |
| TBP | Time-bandwidth product (0.441 for Gaussian) | dimensionless |

---

## Microscopy

| Symbol | Meaning |
|--------|---------|
| NA | Numerical aperture = n·sinα |
| n | Refractive index |
| α | Half-angle of focused cone |
| PSF | Point Spread Function |
| d or d_min | Minimum resolvable distance |
| λ_ex | Excitation wavelength |

---

## CARS

| Symbol | Meaning |
|--------|---------|
| ω_P (or λ_P) | Pump frequency/wavelength |
| ω_S (or λ_S) | Stokes frequency/wavelength |
| ω_AS (or λ_AS) | Anti-Stokes output frequency/wavelength |
| ω_i (or λ_i) | Idler (OPO) |

---

## Transcript-Specific Issues

| Transcript usage | Standard symbol/term | Notes |
|-----------------|---------------------|-------|
| "Blonsky diagram" | Jablonski diagram | Named after Jan Jablonski (Polish physicist) |
| "Gooey phase shift" | Gouy phase shift | Named after Louis-Georges Gouy |
| "Chi" or "Kai" | χ (chi) | Both pronunciations appear in transcript |
| "Brady scattering" or "brain scattering" | Rayleigh scattering | Named after Lord Rayleigh |
| "Brahman scattering" | Raman scattering | Named after C.V. Raman |
| "Andreas" re: CARS | Andreas Zumbusch | First CARS microscopy paper (1999) |
| j vs. i for imaginary unit | Both used: j in engineering contexts (avoids confusion with current i); i in physics contexts. This module uses both — context determines meaning |
| "D is equal to" | D(ω) = ω₀²−ω²−iγω | The detuning denominator in the Lorentz model |
