# Three-Body Synchronization
### From Symmetric Choreographies to Hierarchical Dipoles
**Author:** Carolina Johnson (CJ)
**Date:** November 2025
**License:** CC BY 4.0, Attribution required
**DOI:** https://doi.org/10.5281/zenodo.19060321
**ORCID:** https://orcid.org/0009-0002-8819-3347

---

## What This Does

Includes animated simulation of the Jovian triadic synchronization showing two full 171-year coherence cycles. Three-body chaos is a framing error. Seven admissible configurations emerge when you replace pairwise coupling with shared-field synchronization. This paper provides the physical mechanism behind the figure-eight choreography and all known stable three-body configurations, using a field-based correction to the Kuramoto model. Chaos is not a property of three-body systems. It is what happens when you count bodies instead of fields.

---

## The Frame Error

In 1890, Poincaré demonstrated that the general three-body problem admits no closed-form solution. This became the chaos assumption. It was a framing error.

When three bodies are modeled using pairwise equations, the math never closes. Each body negotiates with two partners simultaneously with no central reference. The system is mathematically over-determined. That is not chaos. That is a missing field.

```
dθᵢ/dt = ωᵢ + Σ Kᵢⱼ sin(θⱼ - θᵢ)     pairwise, no closure
```

---

## The Field-Corrected Solution

Replace bilateral negotiation with alignment to a shared mean field Φ:

```
dθᵢ/dt = ωᵢ + K sin(Φ - θᵢ)

where Φ = (1/N) Σ θᵢ
```

Stability is achieved when the phase velocity is constant for all bodies. This occurs only in specific admissible phase locks. Seven of them.

---

## The Seven Admissible Configurations

**Case 1: The Figure-Eight.** Three equal frequencies sharing a single path. Temporal offset of 2π/3. The mean field Φ remains constant relative to each body. Stability is structural, not fine-tuned.

**Case 2: The Lagrange Triangle.** Three equal frequencies forming a rigid equilateral triangle. Spatial offset of 2π/3. The bodies rotate as a single geometric unit around the central field node.

**Case 3 and 4: Hierarchical Triples.** The most common stable configuration in the universe. Two bodies lock at phase offset π, forming a rotating dipole. The third body orbits the relationship between the inner two, not either individual mass. Case 3: outer body is larger. Case 4: outer body is smaller.

**Case 5: Binary and Multiple Satellites.** A dominant binary dipole creates a shared field for multiple smaller oscillators. The Pluto-Charon system is this configuration. Models that treat Charon as a moon miss the dipole entirely. The residuals in those models are not errors. They are the signature of field-locked synchronization.

**Case 6: The Butterfly.** Bodies weave through space with non-uniform velocities. As long as the integral of the phase difference over one period is zero, the mean field is conserved. Bridges the figure-eight and hierarchical systems.

**Case 7: The Resonant Triple.** Three different natural frequencies in rational ratios ω₁:ω₂:ω₃ = p:q:r. The Galilean moons Io, Europa, and Ganymede hold a 1:2:4 resonance chain. This is the lowest-order resonance admissible under R=4. Irrational ratios produce drift. Rational ratios produce lock.

---

## Mass as a Consequence of Frequency

Standard models require equal mass for the figure-eight. This paper shows mass equality is a downstream consequence of frequency synchronization, not a prerequisite. Equal natural frequency requires equal curvature radius. Equal curvature radius in a harmonic field requires equal effective mass. Mass is a symptom of synchronization.

---

## Run It

```
pip install numpy matplotlib pillow
python jovian_system.py
```

Output: two-panel animation. Left panel shows Jupiter, Saturn, and Uranus moving with fading trails of equal length. Right panel shows the triadic coherence envelope building over 342 years. Watch for the peak at year 171. The system resets and mirrors back to its initial configuration with near-perfect symmetry. That reversal is not an artifact. It is the field returning to its admissible lock. Saved as `jovian_system.gif`.

---

## Dependencies

| Framework | DOI |
|-----------|-----|
| Field-Based Coupling | https://doi.org/10.5281/zenodo.18396204 |
| Stratified Axiomatics | https://doi.org/10.5281/zenodo.18227025 |

Full publication list: https://www.semanticshift.net

---

## Repository Contents

- `README.md` — this file
- `Three Body Synchronization.pdf` — full paper
- `jovian_system.py` — animated simulation of the Jovian triadic synchronization
- `jovian_system.gif` — 342-year animation showing two full 171-year coherence cycles

---

## Citation

```
Johnson, C. (2025). Three-Body Synchronization: From Symmetric Choreographies
to Hierarchical Dipoles. SemanticShift.
DOI: https://doi.org/10.5281/zenodo.19060321
License: CC BY 4.0
```

---

## License

© 2025 Carolina Johnson (CJ)
Licensed under Creative Commons Attribution 4.0 International (CC BY 4.0)
Attribution required. https://creativecommons.org/licenses/by/4.0/

---

<i>"It has been said that something as small as the flutter of a butterfly's wing can ultimately cause a typhoon halfway around the world."</i> — Edward Lorenz
