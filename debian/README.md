# Debian Packaging for dhcpsd

This directory contains the Debian packaging files for dhcpsd.

## Building the Package

```bash
sudo apt build-dep .
gbp buildpackage
```

## Installation

```bash
sudo dpkg -i ../build-area/dhcpsd_*.deb

# Fix any dependency issues
sudo apt-get install -f
```

## Standards Compliance

This packaging follows:
- Debian Policy version 4.6.2
- debhelper compatibility level 13
- FHS (Filesystem Hierarchy Standard)
- systemd integration best practices
