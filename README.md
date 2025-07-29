# Experimental Data: 2D Ship Cross-Section in Regular Waves
This repository contains raw measurement data from a set of two-dimensional wave flume experiments on a ship-like section in beam-sea regular waves. The experiments were performed as part of the Master's thesis of Kristian Reiersen Sundsdal at the Department of Marine Technology, NTNU, and are documented in the paper:

> Sundsdal, K.R., Greco, M., Hanssen, F.-C., & Lugni, C. (2025).
_An experimental investigation of drift forces and coupled-motion effects for a 2D ship cross-section in regular waves._
[Preprint available upon request]

# Summary
These experiments provide a high-quality benchmark dataset for validation of hydrodynamic models and numerical solvers. The test campaign was designed to replicate and expand on the classical experiments of Nojiri and Murayama (1975), using a Lewis-form cross-section in regular waves.

## Scenarios tested:
- A. Fixed model (load measurements in sway, heave, roll)
- B. Free-floating in sway, heave, and roll (3 DOF)
- C. Free-floating with one DOF restricted (2 DOF)

## Use cases include:
- Validating CFD or potential-flow models
- Benchmarking wave-drift force predictions
- Reproducing post-processing techniques
- Designing and planning related model experiments

# Repository structure

The raw data from each test is stored under separate `.csv`-files, all folowing the same naming convention: `XPPH_Rep`. `X` indicates what series the test is a part of, `PP` indicates the applied wave period, `H` indicates the applied wave height, and `_Rep` numbers eventual repetitions. As an example, `3092_2.csv` is the second repetition of test series 3, performed with wave period number 9 wave height number 2.
```
├── data/
│   ├── 1PPH/               # Calibrated waves, without the model
│   ├── 2PPH/               # Scenario A: Fixed model
│   ├── 3PPH/               # Scenario B: Free-floating in sway, heave and roll
│   ├── 4PPH/               # Scenario C: Free-floating in sway and heave
│   ├── 5PPH/               # Scenario C: Free-floating in sway and roll
│   └── 6PPH/               # Scenario C: Free-floating in heave and roll
├── docs/                   
│   ├── experimental_setup.md
│   └── images/
├── README.md
└── LICENSE
```

# Citation
If you use this dataset in your work, please cite the following paper:

``` graphql
@article{Sundsdal2025,
  title={An experimental investigation of drift forces and coupled-motion effects for a 2D ship cross-section in regular waves},
  author={Sundsdal, Kristian R. and Greco, Marilena and Hanssen, Finn-Christian and Lugni, Claudio},
  journal={Ocean Engineeing},
  year={2025}
}
```
# Contact
For questions, collaboration, or requests for the associated preprint:

Kristian Reiersen Sundsdal
📧 k.r.sundsdal@gmail.com