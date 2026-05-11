# Elara: Efficient Lie-group Algorithms for Flexible Robotic Analysis and Control

<div align="center">
  <img src=".assets/elara_logo.png" alt="Elara Logo" width="200"/>
</div>

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![MATLAB Version](https://img.shields.io/badge/MATLAB-R2025b%2B-blue)

## Overview

**Elara** is a MATLAB toolbox for efficient manipulation and control of flexible robotic systems using Lie-group theory and algorithms. This toolbox provides a comprehensive collection of algorithms and computational tools designed to simplify the analysis and control of robots with flexible dynamics, including flexible manipulators, tendon-driven systems, and underactuated mechanisms.

## Purpose

The Elara toolbox addresses the complexity of robotic systems with flexible components by leveraging the mathematical framework of Lie groups and Lie algebras. Key objectives include:

- **Geometric Computation**: Efficient representation and manipulation of rigid body transformations on manifolds
- **Flexible Dynamics**: Algorithms for analyzing systems with elastic deformations and flexible joints
- **Control Design**: Tools for designing controllers that respect the geometry of robotic systems
- **Performance**: Optimized implementations for real-time and offline analysis
- **Accessibility**: User-friendly interfaces for roboticists without deep expertise in differential geometry

## Features

- Lie group and Lie algebra operations (SO(3), SE(3), and extensions for flexible systems)
- Forward and inverse kinematics for flexible manipulators
- Dynamics simulation with flexible components
- Geometric control synthesis
- Trajectory planning and optimization on manifolds
- Visualization and debugging tools

## Installation

1. Clone or download the Elara toolbox:
```matlab
% Add to MATLAB path
addpath('path/to/elara')
addpath(genpath('path/to/elara/src'))
```

2. Verify installation:
```matlab
elara.info()  % Display toolbox information
```

## Quick Start

### Basic Example: SE(3) Transformation
```matlab
% Create a transformation matrix
T = elara.SE3.from_matrix(...);

% Access rotation and translation
R = T.rotation();
p = T.position();

% Compose transformations
T_composed = T1 * T2;
```

### Flexible Manipulator Kinematics
```matlab
% Define manipulator
manipulator = elara.FlexibleManipulator('config.yaml');

% Compute forward kinematics
pose = manipulator.fk(joint_angles, deflections);

% Compute Jacobian
J = manipulator.jacobian(joint_angles);
```

## Citation

If you use the Elara toolbox in your research, please cite:

**BibTeX:**
```bibtex
@software{elara_toolbox,
  author = {Herrmann, M.},
  title = {Elara: Efficient Lie-Group Algorithms for Flexible Robotic Analysis and Control},
  year = {2026},
  url = {https://github.com/ELARA-Toolbox},
  version = {1.0}
}
```

**APA:**
> Herrmann, M. (2026). *Elara: Efficient Lie-group algorithms for flexible robotic analysis and control* [Software]. Retrieved from https://github.com/ELARA-Toolbox

## Documentation

Full documentation is available in the `docs/` directory:
- [Getting Started Guide](docs/getting_started.md)
- [API Reference](docs/api/)
- [Examples](examples/)
- [Theory](docs/theory/)

## Requirements

- MATLAB R2020a or later
- CasADi ... TODO add how to install


## Examples

See the `examples/` directory for demonstration scripts:
- Basic Lie group operations
- Flexible manipulator kinematics and dynamics
- Control synthesis and simulation
- Trajectory planning

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

## Authors

- [Your Name/Organization]

## Acknowledgments

This toolbox builds on the theoretical foundations of differential geometry and Lie group theory applied to robotics. Special thanks to the robotics and control communities for inspiration and feedback.

## Contact & Support

For questions, issues, or feature requests:
- Open an issue on GitHub
- Contact: [your-email@example.com]

---

**Note:** This is a placeholder version. Please update the following fields with actual information:
- Author names and affiliations
- Journal/conference details and DOI
- GitHub repository URL
- Contact information
- Links to actual documentation files
