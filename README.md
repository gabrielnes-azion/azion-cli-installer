# Azion CLI Installer

One-line installer for the [Azion CLI](https://www.azion.com/en/documentation/products/azion-cli/overview/).

## Install

```bash
curl -fsSL https://cli.azion.app/install.sh | bash
```

### Pin a specific version

```bash
AZION_VERSION=4.16.0 curl -fsSL https://cli.azion.app/install.sh | bash
```

### Custom install directory (Linux/FreeBSD only)

```bash
AZION_INSTALL_DIR=/usr/local/bin curl -fsSL https://cli.azion.app/install.sh | bash
```

## How it works

| Platform | Method |
|----------|--------|
| macOS (with Homebrew) | `brew install azion` |
| Linux (deb-based) | Downloads `.deb` and installs via `dpkg` |
| Linux (rpm-based) | Downloads `.rpm` and installs via `dnf`/`yum` |
| Linux (Alpine) | Downloads `.apk` and installs via `apk` |
| Other | Downloads binary zip to `~/.azion/bin` |
