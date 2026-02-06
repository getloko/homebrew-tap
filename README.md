# Homebrew Tap for LoKO

<div align="center">
  <img src="https://avatars.githubusercontent.com/u/257918568?s=200" alt="LoKO Logo" width="200" height="200">
</div>

Official Homebrew tap for [LoKO](https://github.com/getloko/loko) - Local Kubernetes Environment Manager.

## Installation

**Recommended (two-step)**:
```bash
brew tap getloko/tap
brew install loko
```

<details>
<summary>Alternative: One-liner installation</summary>

```bash
brew install getloko/tap/loko
```

Note: This skips the explicit tap step but results in a redundant-looking command.
</details>

## Usage

After installation, the `loko` command will be available:

```bash
# Verify installation
loko --version
loko --help

# Example usage
loko catalog list
loko deploy myapp
```

## Upgrading

```bash
# Update tap and upgrade loko
brew upgrade loko
```

## Uninstallation

```bash
brew uninstall loko
brew untap getloko/tap
```

## About LoKO

LoKO (Local Kubernetes Oasis) simplifies local Kubernetes development with Kind. It provides:

- **Workload Catalog**: Pre-configured Helm deployments for common services
- **Environment Management**: Easy cluster creation and configuration
- **Template System**: Customizable Kubernetes manifests
- **Credential Management**: Secure handling of secrets and credentials

For more information, visit the [main repository](https://github.com/getloko/loko).

## Package Information

- **Package Name**: `loko-k8s` (on PyPI)
- **Formula Name**: `loko` (Homebrew)
- **License**: MIT
- **Python Version**: 3.10+

## Alternative Installation Methods

If you prefer not to use Homebrew:

```bash
# Using pip
pip install loko-k8s

# Using uv
uv tool install loko-k8s

# From source
git clone https://github.com/getloko/loko.git
cd loko
uv sync
uv run loko --help
```

## Issues

For issues related to:
- **Formula/installation**: [Report here](https://github.com/getloko/loko-homebrew/issues)
- **LoKO functionality**: [Report here](https://github.com/getloko/loko/issues)

## Contributing

Contributions are welcome! If you find an issue with the formula or have suggestions for improvement, please open an issue or pull request.
