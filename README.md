# _Optical and transport anisotropies in spin-textured altermagnets_: Code for the paper

This repo has two jobs:

1. **Analytics (SymPy notebooks)** that reproduce and *test* the key algebra in the appendix:
   - Weyl (total) symmetrization expansions
   - First-order projection \(PVP\) to the low-energy doublet
   - Second-order Schrieffer–Wolff (SW) effective Hamiltonian checks

2. **Paper plots (Matplotlib notebooks + exported figures)** used in the manuscript.

---

## Repository structure

```
.
├── analytics
│   ├── schrieffer_wolff.ipynb
│   ├── schrieffer_wolff_secondorder.ipynb
│   └── weyl.ipynb
└── paper_plots
├── spiral.ipynb
└── paper_plot_style.mplstyle

````

### `analytics/`
Notebooks focused on **symbolic derivations** with SymPy. They are written as “executable appendix” material: each notebook ends with `assert`-style checks that expressions match the closed-form results quoted in the paper.

- `weyl.ipynb`  
  Implements the Weyl-symmetrized expansions used in the long-wavelength truncation, including the \(O\!\left((\mathbf A^\perp)^2\right)\) metric terms.

- `schrieffer_wolff.ipynb`  
  Builds the 4×4 model, defines the low-energy projector \(P\), and verifies the **first-order** projected Hamiltonian \(PVP\) for the relevant d-wave (and related) sectors.

- `schrieffer_wolff_secondorder.ipynb`  
  Verifies the **second-order Schrieffer–Wolff correction**:

### `paper_plots/`
Notebooks and exported figures used in the manuscript.

- `spiral.ipynb`  
  Produces the spiral-frame calculations and generates the paper figures in this folder.

- `paper_plot_style.mplstyle`  
  Matplotlib style file used to keep typography, line widths, tick sizes, etc. consistent.
  
---

## Citation

If you use or adapt this code for related work, please cite the associated manuscript and link back to this repository in your documentation.
