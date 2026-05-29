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
@software{elara_toolbox,
  author = {Herrmann, Maximilian},
  title = {Elara: Efficient Lie-Group Algorithms for Flexible Robotic Analysis and Control},
  year = {2026},
  url = {https://github.com/ELARA-Toolbox},
  version = {0.1}
}
```

**APA:**
> Herrmann, M. (2026). *Elara: Efficient Lie-group algorithms for flexible robotic analysis and control* [Software]. Retrieved from https://github.com/ELARA-Toolbox

## License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

## Authors

- Maximilian Herrmann [TUM, Chair of Automatic Control]
- Leander Pfeiffer [TUM, Chair of Automatic Control]

## Acknowledgments

This toolbox builds on the theoretical foundations of differential geometry and Lie group theory applied to robotics. Special thanks to the robotics and control communities for inspiration and feedback.

## Contact & Support

For questions, issues, or feature requests:

- Open an issue on GitHub
- Contact: [maximilian.herrmann@tum.de, leander.pfeiffer@tum.de]
