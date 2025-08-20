# Test14 Project

A sample ASIC design project demonstrating RTL development, verification, and synthesis workflows using open-source EDA tools.

## Overview

This project serves as a template and testing ground for digital ASIC design methodologies. It includes examples of:

- RTL design using SystemVerilog/Verilog
- Verification using cocotb and pyuvm
- Synthesis with Yosys
- Physical implementation with OpenLane/LibreLane
- Integration with Caravel SoC framework

## Project Structure

```
test14/
├── rtl/                    # RTL source files
├── tb/                     # Testbench files
├── sim/                    # Simulation results
├── syn/                    # Synthesis outputs
├── config/                 # Configuration files
├── docs/                   # Documentation
└── scripts/                # Build and automation scripts
```

## Getting Started

### Prerequisites

- Python 3.8+
- Yosys synthesis suite
- Verilator or Icarus Verilog
- cocotb verification framework
- OpenLane (for physical implementation)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/kanndil/test14.git
   cd test14
   ```

2. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up the environment:
   ```bash
   source setup_env.sh
   ```

## Usage

### RTL Development

RTL modules are located in the `rtl/` directory. Follow the coding guidelines:

- Use SystemVerilog-2017 subset compatible with Yosys
- Apply consistent naming conventions (snake_case for signals, PascalCase for modules)
- Include proper reset handling and clock domain management
- Ensure synthesis-friendly constructs only

### Verification

Run verification using cocotb:

```bash
make -C tb/ MODULE=test_module
```

### Synthesis

Synthesize RTL using Yosys:

```bash
make synthesize TOP_MODULE=YourModule
```

### Physical Implementation

Run OpenLane flow:

```bash
make openlane CONFIG=config/your_config.json
```

## Design Modules

### Core Modules

- **Module1**: Brief description of functionality
- **Module2**: Brief description of functionality
- **Module3**: Brief description of functionality

### Verification Status

| Module | RTL Complete | Verification | Synthesis | Physical |
|--------|-------------|-------------|-----------|----------|
| Module1| ✅          | ✅          | ✅        | ⏳       |
| Module2| ✅          | ⏳          | ❌        | ❌       |
| Module3| ⏳          | ❌          | ❌        | ❌       |

## Documentation

- [Design Specification](docs/design_spec.md)
- [Verification Plan](docs/verification_plan.md)
- [Integration Guide](docs/integration_guide.md)
- [API Reference](docs/api_reference.md)

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Coding Standards

- Follow the RTL coding guidelines in `docs/coding_standards.md`
- Ensure all code passes linting checks
- Include comprehensive testbenches for new modules
- Update documentation for any interface changes

## Testing

Run the complete test suite:

```bash
make test
```

Run specific tests:

```bash
make test TEST=test_specific_module
```

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built using open-source EDA tools
- Leverages the Caravel SoC framework
- Inspired by the open-source silicon community

## Contact

- Project Maintainer: [Your Name](mailto:your.email@example.com)
- Repository: [https://github.com/kanndil/test14](https://github.com/kanndil/test14)
- Issues: [https://github.com/kanndil/test14/issues](https://github.com/kanndil/test14/issues)

---

*This is a dummy README file created for demonstration purposes. Please update the content to reflect your actual project details.*