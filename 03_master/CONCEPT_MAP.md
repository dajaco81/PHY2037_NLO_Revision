# PHY2037 Concept Map

How all the key ideas in the module connect to each other.

---

## Central Axis: P = ε₀χE

Everything in the course flows from this single equation. χ is the material property; P is the response we use to understand and image materials.

```
                        ┌─────────────────────┐
                        │   ELECTRIC FIELD E   │
                        │   (from laser/light) │
                        └──────────┬──────────┘
                                   │ drives
                                   ▼
                     ┌─────────────────────────┐
                     │ INDUCED POLARISATION P   │
                     │  = ε₀χE (linear)        │
                     │  = ε₀[χ₁E+χ₂E²+χ₃E³…] │
                     └──────────┬──────────────┘
                                │ contains
                         ┌──────▼──────┐
                         │      χ      │
                         │ susceptibility│
                         └──────┬──────┘
              ┌─────────────────┼─────────────────┐
              │                 │                 │
              ▼                 ▼                 ▼
       χ is frequency-    χ is a tensor     χ can be expanded
       dependent          (not scalar)      as a power series
              │                                   │
              ▼                                   ▼
       Lorentz model                     χ⁽²⁾ and χ⁽³⁾ terms
       → χ(ω) derivation                 → nonlinear optics
```

---

## The Lorentz Model

```
     Harmonic oscillator    +   EM wave driving   →   χ(ω)
     (waves & optics)           (Maxwell's eqs)        (frequency-dependent susceptibility)
                                       │
                                       ▼
                         POLARISATION TIMESCALES
                         
     femtosecond          picosecond          microsecond
     electronic           vibrational          orientational
     (UV/visible)         (infrared)           (microwave)
         │                    │
         ▼                    ▼
     Colour/fluorescence  Molecular fingerprint
     NOT chemically       CHEMICALLY SPECIFIC
     specific             (C-H, C=O, etc.)
         │                    │
         ▼                    ▼
     Dyes, labels         IR absorption
     H&E staining         Raman scattering
```

---

## Nonlinear Extension: Anharmonic Potential

```
     Small displacement:        Large displacement:
     parabolic potential        anharmonic potential
     linear χ                  χ₁ + χ₂E + χ₃E² + …
           │                         │
           ▼                         ▼
     Single frequency         Multiple frequencies
     response at ω            response at 2ω, 3ω, ω₁±ω₂…
                                      │
                        ┌─────────────┼──────────────┐
                        │             │              │
                        ▼             ▼              ▼
                     SHG           THG           4WM/CARS
                  (2ω output)   (3ω output)    (2ω₁−ω₂)
```

---

## Phase Matching Chain

```
     Nonlinear processes generate P at new frequencies
                     │
                     ▼
     P acts as source in wave equation
                     │
                     ▼
     For signal to build up: all sources must be in phase
     (constructive interference along propagation axis)
                     │
                     ▼
     Phase matching: Δk = k₃ − k₁ − k₂ = 0
                     │
     But dispersion makes this hard:
     n(2ω) > n(ω) for normal dispersion → Δk ≠ 0
                     │
                     ▼
     Solutions:
     ├─ Angle tuning (birefringent crystal)
     ├─ Temperature tuning (LiNbO₃)
     └─ Periodic poling / PPLN (quasi-PM)
                     │
     Special case — tight microscope focus:
     ├─ Range of k-vectors relaxes strict PM
     ├─ Gouy phase shift adds ±π/2 per beam
     ├─ SHG: L < λ/2 (achievable) → works
     ├─ THG: L < λ/3 (too tight for bulk) → interfaces only
     └─ CARS (2ω₁−ω₂): Gouy partially cancels → works in bulk
```

---

## The Core Imaging Problem and NLO Solution

```
     CONVENTIONAL IMAGING TRADEOFFS
     
     Short λ (blue) ──────► Good resolution (d = λ/2NA)
                     BUT ──► High scattering (I∝1/λ⁴)
     
     Long λ (IR) ──────────► Deep penetration
                     BUT ──► Poor resolution
                             AND wrong wavelength for contrast mechanism
     
     Chemical contrast ────► Dictated by molecule (e.g., 400 nm)
                             Can't change it without labelling
     ─────────────────────────────────────────────────────────
     
     NONLINEAR OPTICS SOLUTIONS
     
     2PEF (χ⁽³⁾ — two photon absorption):
     ├─ Excite with 2λ (IR) → 16× less scattering
     ├─ Signal ∝ I² → only at focus → no pinhole
     └─ Resolution: d_2P = 0.61√2·λ/NA (≈1.41× 1PEF, not 2×)
     
     SHG (χ⁽²⁾ — second harmonic):
     ├─ Non-centrosymmetric only → collagen, myosin
     ├─ Parametric → phase matching (just works in focus)
     └─ Label-free, no photobleaching
     
     CARS/SRS (χ⁽³⁾ — coherent Raman):
     ├─ Chemical specificity from vibrational fingerprint
     ├─ Much faster than spontaneous Raman
     ├─ CARS: has NR background; SRS: background-free
     └─ Need ps pulses for spectral selectivity
```

---

## Laser Pulses

```
     Why pulsed lasers?
     
     Required I ≈ 3×10²⁰ W/m²
              │
     Spatial focus:  A = (λ/2)² ≈ 10⁻¹³ m² → P_CW ≈ 30 MW (too much!)
              │
     Temporal squeezing:
     ├─ NLO signal ∝ I² or I³ → peak intensity matters, not average
     ├─ Same average power → 10⁸× higher peak power (1 kHz vs 80 MHz example)
     └─ Side effect: bandwidth ↔ pulse width (TBP = 0.441)
     
     Pulse types:
     ├─ Femtosecond (KLM Ti:Sapphire) → max peak intensity → 2PEF, SHG, THG
     └─ Picosecond (SESAM) → narrow bandwidth → CARS, SRS spectroscopy
     
     Frequency conversion:
     ├─ SHG crystal: λ → λ/2
     └─ OPO: pump → signal + idler (1/λ_P = 1/λ_S + 1/λ_i)
```

---

## Applications Chain

```
     Phase matching derivation (L10)
              │
              ▼
     EPI-CARS: sub-λ objects only give backward signal (L15, L18)
              │
              ▼
     Nanoparticle drug delivery imaging (L18)
     Microplastics in organisms (L18)
     
     CARS/SRS (L16) 
              │
              ▼
     Virtual H&E staining + AI → cancer diagnosis (L18)
     Drug diffusion through skin (L18)
     Lipid imaging in brain/skin (L16, L18)
     
     SHG (L15)
              │
              ▼
     Collagen structure in cartilage / tumour (L15, L18)
     Myosin in muscle disease (L15, L18)
     
     2PEF (L14)
              │
              ▼
     Deep tissue imaging (L14, L15)
     Neuronal imaging to 800 µm (L14)
```

---

## Key Numbers to Remember

| Quantity | Value |
|----------|-------|
| Bohr radius | a₀ ≈ 0.53 Å |
| Atomic field strength | E_at ≈ 5×10¹¹ V/m |
| Required intensity for NLO | ~3×10²⁰ W/m² |
| χ⁽²⁾ (typical) | ~2×10⁻¹² m/V |
| χ⁽³⁾ (typical) | ~4×10⁻²⁴ m²/V² |
| Time-bandwidth product (Gaussian) | 0.441 |
| Scattering reduction per factor-2 in λ | 16× (factor 2⁴) |
| CARS: CH₂ stretch | ~2845–2900 cm⁻¹ |
| C=O stretch (IR) | ~1700 cm⁻¹ |
| C–D stretch (silent region) | ~2100 cm⁻¹ |
| Blue light | ~400–490 nm |
| Green light | ~500 nm |
| Red light | ~600–680 nm |
