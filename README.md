# Calamares Settings for Cutefish OS

This package provides Cutefish OS specific configuration files for the Calamares system installer.

## Overview

Following Calamares official recommendation to separate distribution configuration from the main program, this package contains:

- Cutefish OS branding (logos, colors, QML interface)
- Module configurations for installation process
- Settings for partitioning, users, packages, etc.

## Installation

### From source

```bash
mkdir build
cd build
cmake ..
make
sudo make install
```

### Building Debian package

```bash
dpkg-buildpackage -us -uc -b
```

## Package Structure

- `cutefish_config/settings.conf` - Main Calamares configuration
- `cutefish_config/branding/cutefishos/` - Branding files (logos, QML)
- `cutefish_config/modules/` - Module configuration files

## Dependencies

- `calamares` (>= 3.3.0)

## Usage

This package should be installed alongside `cutefish-calamares` to provide a complete Cutefish OS installation experience.

## License

- Configuration files: GPL-3.0+
- Branding files: CC-BY-SA-4.0