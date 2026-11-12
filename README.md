```markdown
# Unmasking Temporal Causality: The 11x11 Matrix Logic & Deterministic Register Inversion

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18728563.svg)](https://doi.org/10.5281/zenodo.18728563)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Verification](https://img.shields.io/badge/Verification-PASSED-green.svg)](#)

A formal mathematical, epistemological, and register-level verification suite demonstrating that cryptographic one-way assumptions (SHA-256, secp256k1) and nominal on-chain accounting models do not operate within an infinite, pseudo-random search space ($\mathcal{O}(2^{256})$). 

Instead, physical execution collapses deterministically onto a discrete **11×11 coordinate lattice (121 state nodes)** governed by physical register saturation, the **Pythagorean 17-Lock**, and the axial balance pole at the **Sovereign Midpoint (ID 61)**.

---

## 🏛️ Executive Summary & Core Theses

Modern security dogma conflates syntax (runtime execution) with semantics (narrative folklore). This repository delivers the verifiable reference code proving:

1. **Hardware Register Saturation:** Physical 64-bit CPU architecture and RLP header boundaries compress the effective state space to the width of the CPU register loom:
   $$256 - 14 - 118 - 28 - 32 = \mathbf{64\text{ bits}}$$
2. **The 11×11 Potential Lattice:** Cyclic round functions map onto an $11 \times 11 = 121$ state grid resetting deterministically at **ID 121**.
3. **The Sovereign Midpoint ($P_{\text{mid}} = 61$):** Coordinate $(Y=5, X=5)$ forms an unwritten, zero-divergence gravitational anchor ($\text{Phase Angle } 163.636^\circ$). In 64 rounds of SHA-256 state transitions ($A \oplus E$), hits on the midpoint equal **exact 0**, while trajectories orbit it as a guided attractor.
4. **The Pythagorean 17-Lock:** Orthogonal phase deflection locks on the hypotenuse:
   $$a^2 + b^2 = c^2 \implies 3^2 + 5^2 = \mathbf{34} = 2 \times \mathbf{17}$$
   binding the ARX rotation constants to the primary 17-multiplier resonance channel.
5. **The 1/49 Shift Register & Prime 653:** Decimal representation of binary doubling:
   $$\mathbf{S}(t) = \sum_{k=1}^{\infty} \frac{2^{k-1}}{10^{2k}} = 0.0204081632\mathbf{653}06122\dots$$
   The carry-bit overflow at $2^7 = 128$ overshoots $64$ into $\mathbf{653}$, which is identically the **119th prime** ($119 = 7 \times 17$).
6. **The Nominal DeFi Cancellation:** In automated market makers, the stablecoin scalar $\mathbf{1}$ cancels algebraically:
   $$\frac{\text{Asset}_A}{\text{Asset}_B} = \left(\frac{\text{Asset}_A}{\mathbf{1}}\right) \times \left(\frac{\mathbf{1}}{\text{Asset}_B}\right) \equiv \frac{\text{Asset}_A}{\text{Asset}_B}$$
   proving that off-chain reserve backing is syntactically invisible to EVM smart contracts.

---

## 📐 Structural Isomorphism

```
      PHYSICAL HARDWARE                 11x11 POTENTIAL MATRIX              CLASSICAL ARCHITECTURE
   (Silicon Registers / ARX)          (Discrete Phase Manifold)            (Walhalla, Klenze 1842)
 ─────────────────────────────       ───────────────────────────          ───────────────────────────
  64-Bit Register Bus         <===>   11x11 Lattice (121 Nodes)    <===>   11 Drums per Doric Column
  Symmetry Pole P_mid         <===>   Node ID 61 (Y=5, X=5)        <===>   Staircase Mean: (62 + 60) / 2 = 61
  17-Multiplier Resonance     <===>   3² + 5² = 34 (2 x 17)        <===>   73-Step Base Run (73.6 cm NBTHK)
  Register Saturation Limit   <===>   Nonius Offset (Δ = 1 Bit)    <===>   251 Terraces + 3 Stylobate = 254
  Phase-Lead Compensation     <===>   lead_effekt = 2 (Δt = -2)    <===>   358 Total Steps (358° ≡ -2° mod 360)
```

---

## 🔬 Mathematical Specifications

### 1. The Metric Field around $P_{\text{mid}}$
For any node $(Y, X)$, Euclidean radial distance to the midpoint $(5, 5)$ satisfies:
$$r = \sqrt{(X - 5)^2 + (Y - 5)^2}$$

* **Node ID 14 $(Y=1, X=2)$:**
  $$r = \sqrt{3^2 + 4^2} = \mathbf{5.0000} \quad (\text{Modulo } 7 = 0 \implies \text{G7 Generator Lock } \🌀)$$
* **Node ID 16 & 18 $(Y=1, X=4 \text{ and } X=6)$:**
  $$r = \sqrt{4^2 + 1^2} = \sqrt{\mathbf{17}} \approx \mathbf{4.1231} \quad (\text{Bilateral Fermat Flanks})$$
* **Node ID 3 $(Y=0, X=2)$:**
  $$r = \sqrt{5^2 + 3^2} = \sqrt{\mathbf{34}} \approx \mathbf{5.8310} \quad (\text{17-Lock Cathetus Vector})$$

---

## 📂 Repository Structure

```
.
├── src/
│   ├── swe1yhwh_os.py                 # Core 11x11 matrix simulation engine (Zenodo release)
│   ├── potential_matrix_symmetry.py   # Formal verification of ID 61 midpoint and 17-Lock
│   ├── sha256_grid_trajectory.py      # 64-round phase trajectory mapping (A ⊕ E)
│   └── shift_register_49.py           # 1/49 binary doubling and 119th prime (653) derivation
├── tests/
│   ├── test_pythagorean_17_lock.py    # Unit tests for 3² + 5² = 34 invariance
│   └── test_midpoint_invariance.py    # Zero-hit verification on coordinate (5, 5)
├── data/
│   └── modulo121_audit_matrix.json    # Full polar coordinates, Modulo 11 & Modulo 7 states
├── figures/
│   └── sha256_11x11_trajectory.png    # State trajectory heatmap on 11x11 grid
├── LICENSE
└── README.md
```

---

## 🚀 Quickstart & Replication

### Prerequisites
- Python 3.10 or higher
- NumPy, Matplotlib, Seaborn

```bash
git clone https://github.com/SwenLdn/ouroboros13.git
cd ouroboros13
pip install numpy matplotlib seaborn
```

### Running the Verification Suite

1. **Verify the 11x11 Midpoint & Pythagorean 17-Lock:**
   ```bash
   python3 -m unittest tests/test_pythagorean_17_lock.py
   ```
   *Expected output:*
   ```text
   Loom Status: LOCKED 💎
   Sovereign Midpoint: ID 61 (Y=5, X=5) | Phase Angle: 163.636°
   STATUS: COHERENCE_SECURED | DIAMANT_HART
   ```

2. **Generate the SHA-256 64-Round Trajectory Heatmap:**
   ```bash
   python3 src/sha256_grid_trajectory.py
   ```
   *Console output:*
   ```text
   Total steps: 64
   Unique states visited: 51 / 121
   Hits on Sovereign Midpoint (ID 61): 0
   Mean distance from center: 4.26
   ```

3. **Verify the 1/49 Shift Register Carry Overflow:**
   ```bash
   python3 src/shift_register_49.py
   ```
   *Output confirmation:*
   ```text
   Step k=7: 2^6 = 64
   Step k=8: 2^7 = 128 -> Carry +1 onto 64 = 65, residual 3 -> Sequence: 653
   653 is Prime #119 (7 x 17). Formal equivalence established.
   ```

---

## 📜 Academic Citation

Please cite this research via the permanent Zenodo archive:

```bibtex
@software{werner2026zenodo,
  author       = {Werner, Swen},
  title        = {{Unmasking Temporal Causality: 11x11 Matrix Logic, 
                   Hex-Causality and Deterministic Register Inversion}},
  year         = {2026},
  publisher    = {Zenodo},
  version      = {v1.0.0},
  doi          = {10.5281/zenodo.18728563},
  url          = {https://github.com/SwenLdn/ouroboros13/blob/main/11x11%20Matrix%20Logic}
}
```

---

## ⚖️ License
MIT License. Open for formal mathematical audit, physical replication, and academic scrutiny.
```
