# Inconsistency Log

Contradictions or variations between lectures that could cause confusion.

---

## I01 — Rayleigh Criterion Constant

**Issue:** The lecturer uses 1.22λ/D for the Airy disk radius, 0.61λ/NA for the Rayleigh resolution criterion, and 0.5λ/NA for the Abbe limit interchangeably in different lectures.

**Details:**
- L04: "it's this equation here" (hard to determine exact value from transcript; both 0.61 and 1.61 mentioned)
- The standard physical values are: Airy disk radius r = 1.22λ/D; Rayleigh criterion d = 0.61λ/NA; Abbe limit d = 0.5λ/NA

**Resolution:** All three arise from the same derivation with slightly different definitions. Use **d = 0.61λ/NA** (Rayleigh criterion) as the standard for this module unless otherwise specified. The derivation method is the same regardless of which constant appears.

---

## I02 — FWHM Derivation: Amplitude vs. Intensity Gaussian

**Issue:** In L02 the FWHM formula FWHM = 2√(2ln2)σ is derived for an amplitude Gaussian. In L14, the time-bandwidth product uses an intensity Gaussian where the FWHM formula is 2σ√(ln2) (narrower by √2).

**Details:**
- Amplitude Gaussian: f(t) = exp(−t²/2σ²) → FWHM = 2√(2ln2)σ ≈ 2.355σ
- Intensity Gaussian: I(t) = exp(−t²/σ²) [note different convention, σ here is not σ/√2 of the amplitude] → FWHM = 2√(ln2)σ ≈ 1.665σ

**Resolution:** For pulse characterisation (τ_p) we always use the intensity FWHM (you measure intensity on a photodetector). For the spatial PSF we typically state both. Make sure to state which you're using. The TBP derivation in L14 uses intensity FWHMs consistently.

---

## I03 — Jitter Specification

**Issue:** L17 states electronic synchronisation achieves "a few tens of femtoseconds" of jitter and says "20 femtoseconds". However, the 1 kHz laser example in L12 implies pulses are 100 fs wide, and in L17 says a 20 fs jitter on 100 fs pulses is "20% overlap, a bit rubbish".

**Resolution:** No contradiction — these are consistent. 20 fs jitter with 100 fs pulses means 80% overlap (acceptable for some applications, not ideal for femtosecond CARS). The optical injection locking method (<5 fs jitter) resolves this.

---

## I04 — Coherence Length Definition

**Issue:** "Coherence length" appears to be used informally in the transcripts. The standard definition is L_c = π/Δk (position of first zero of sinc²).

**Resolution:** Use L_c = π/Δk consistently. This is where ΔkL_c/2 = π/2, giving sinc²(π/2) = 4/π² ≈ 0.4 (not zero — the first zero is at ΔkL/2 = π, i.e., L = 2π/Δk). Some texts define L_c differently. The exam derivation produces the sinc² function and asks where it peaks — this is at Δk = 0 or L → 0 limit.

---

## I05 — Spring Constant Values

**Issue:** L07 quotes vibrational spring constants as "five times ten to the five grams per second squared" for a single bond.

**Resolution:** This is a unit error in the transcript. Standard values are approximately:
- Single bond: k ≈ 5×10² N/m = 500 N/m
- Double bond: k ≈ 10³ N/m = 1000 N/m
- Triple bond: k ≈ 1.5×10³ N/m = 1500 N/m

These give reasonable vibrational frequencies (~1000–3000 cm⁻¹) for C–H, C=O, C≡N bonds. The transcript values appear to be in cgs units (g·s⁻²) — 5×10⁵ g/s² = 500 N/m after unit conversion. [INFERRED CORRECTION from standard references.]

---

## I06 — D(2ω) in Perturbation Theory

**Issue:** The denominator in the second-order SHG susceptibility: various forms appear in the transcript — "D(2ω)" and "D(ω)²". The correct result is a product of both.

**Resolution:** The correct χ⁽²⁾ for SHG has the form:
$$\chi^{(2)}(2\omega;\omega,\omega) \propto \frac{1}{D(\omega)^2 \cdot D(2\omega)}$$

Two factors of D(ω) from the squared linear response r₁², and one factor of D(2ω) from the second-order equation of motion at the frequency 2ω.
