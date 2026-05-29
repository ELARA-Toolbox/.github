<div align="center">
  <img src=".assets/banner.png" alt="Elara: Efficient Lie-group Algorithms for Flexible Robotic Analysis and Control" style="width:100%;height:auto;max-width:100%;"/>
</div>

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![MATLAB Version](https://img.shields.io/badge/MATLAB-R2025b%2B-blue)
![Work in Progress](https://img.shields.io/badge/status-WIP-orange)

## Overview

**Elara** is a MATLAB toolbox for efficient simulation and integration of rigid-flexible robotic systems. It can handle multibody systems with a tree structure. Each link can be either rigid or flexible, and each joint can be actuated. Additionally, flexible links can be tendon-actuated, allowing for modeling of custom continuum-robot systems.

The simulation is based on the Lie-Group Variational Integrator proposed by Herrmann and Kotyczka and features superior numerical stability even for longer time-step choices. The same integrator also serves as the foundation of the optimal control approaches built in the toolbox.

## Features

- **Efficient simulation of rigid and flexible-link dynamics**
- **Optimal control framework for trajectory planning**
-- **Optional symbolic implementation using CasADi** (for fast derivatives)

## Implementation

The current implementation is available in MATLAB (verified in R2025b) in the [Elara repository](https://github.com/ELARA-Toolbox/ELARA).

> ⚠️ **Work in progress: We are planning some further improvements to increase accessibility. A full release is scheduled for July 2026**

## Citation

If you use the Elara toolbox in your research, please cite:

**BibTeX:**

```bibtex
@article{HK24,
  title = {Relative-Kinematic Formulation of Geometrically Exact Beam Dynamics Based on {{Lie}} Group Variational Integrators},
  author = {Herrmann, Maximilian and Kotyczka, Paul},
  year = 2024,
  month = dec,
  journal = {Computer Methods in Applied Mechanics and Engineering},
  volume = {432},
  pages = {117367},
  issn = {00457825},
  doi = {10.1016/j.cma.2024.117367},
}
@inproceedings{HPK26,
  title = {Discrete {{Geometric Modeling}} and {{Extended State Estimation}} of {{Continuum Robots}}},
  booktitle = {IFAC World Congress},
  author = {Herrmann, Maximilian and Pfeiffer, Leander and Kotyczka, Paul},
  year = 2026,
  address = {Busan},
  }
```

**APA:**

> Herrmann, M., & Kotyczka, P. (2024). Relative-kinematic formulation of geometrically exact beam dynamics based on Lie group variational integrators. Computer Methods in Applied Mechanics and Engineering, 432, 117367. https://doi.org/10.1016/j.cma.2024.117367

> Herrmann, M., Pfeiffer, L., & Kotyczka, P. (2026). Discrete Geometric Modeling and Extended State Estimation of Continuum Robots. IFAC World Congress.

## License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

## Authors

- Maximilian Herrmann [TUM, Chair of Automatic Control]
- Leander Pfeiffer [TUM, Chair of Automatic Control]

## Contact & Support

For questions, issues, or feature requests:

- Open an issue on GitHub
- Contact: [maximilian.herrmann@tum.de, leander.pfeiffer@tum.de]
