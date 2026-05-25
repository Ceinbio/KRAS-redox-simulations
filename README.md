# Oncogenic Cysteine Mutations Rewire KRAS Redox Chemistry and Impair GAP-Mediated Shutoff

This repository contains the molecular dynamics (MD) simulation datasets, analysis scripts, and supporting files associated with the study:

> **Oncogenic cysteine mutations rewire KRAS redox chemistry and impair GAP-mediated shutoff**

## Overview

KRAS is one of the most frequently mutated oncogenes in human cancer. In this work, we investigated how oncogenic cysteine substitutions and their distinct redox states alter KRAS conformational dynamics.

Using all-atom molecular dynamics simulations, we explored the structural and dynamical consequences of introducing cysteine residues at positions 12 and 13 under multiple oxidation states.

All systems were simulated in the GDP/Mg²⁺-bound state.

---

## Simulated Systems

The following KRAS variants and cysteine oxidation states were simulated:

| KRAS Variant | C12 State | C13 State | C118 State |
|---|---|---|---|
| WT   | –     | –     | -SH |
| WT   | –     | –     | -S⁻ |
| G12C | -SH   | –     | -SH |
| G12C | -S⁻   | –     | -SH |
| G12C | -SOH  | –     | -SH |
| G12C | -SO⁻  | –     | -SH |
| G12C | -SNO  | –     | -SH |
| G13C | –     | -SH   | -SH |
| G13C | –     | -S⁻   | -SH |
| G13C | –     | -SOH  | -SH |
| G13C | –     | -SO⁻  | -SH |
| G13C | –     | -SNO  | -SH |

### Cysteine Redox States

| State | Description |
|---|---|
| `-SH` | Thiol |
| `-S⁻` | Thiolate |
| `-SOH` | Sulfenic acid |
| `-SO⁻` | Sulfenate |
| `-SNO` | S-nitrosothiol |

---

## Repository Structure

```text
.
├── systems/            # Initial coordinates, topologies, and parameter files
├── trajectories/       # Production MD trajectories
└── README.md
```

---

## Simulation Details

- **Protein:** KRAS GDP/Mg²⁺-bound state
- **Force field:** ff14SB
- **Water model:** TIP3P
- **Ions:** Neutralizing counterions and physiological salt concentration
- **MD engine:** AMBER
- **Temperature:** 300 K
- **Pressure:** 1 atm
- **Boundary conditions:** Periodic boundary conditions

---

## Analyses Performed

Representative analyses included:

- RMSD and RMSF
- Switch I / Switch II conformational dynamics
- Hydrogen-bond and salt-bridge analysis
- Principal component analysis (PCA)
- Free-energy landscapes
- GAP interaction interface characterization
- Redox-state-dependent structural rearrangements

---

## Citation

If you use this repository or associated datasets, please cite:

```text
Patra, S. et al.
Oncogenic cysteine mutations rewire KRAS redox chemistry and impair GAP-mediated shutoff.
```

---

## Contact

Ari Zeida 
Facultad de Medicina / CEINBIO – Universidad de la República  
Montevideo, Uruguay
