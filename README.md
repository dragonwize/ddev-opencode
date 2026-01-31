[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/dragonwize/ddev-opencode/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/dragonwize/ddev-opencode/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/dragonwize/ddev-opencode)](https://github.com/dragonwize/ddev-opencode/commits)
[![release](https://img.shields.io/github/v/release/dragonwize/ddev-opencode)](https://github.com/dragonwize/ddev-opencode/releases/latest)

# DDEV Opencode

## Overview

This add-on integrates Opencode into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get dragonwize/ddev-opencode
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Opencode |
| `ddev logs -s opencode` | Check Opencode logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.opencode --opencode-docker-image="ddev/ddev-utilities:latest"
ddev add-on get dragonwize/ddev-opencode
ddev restart
```

Make sure to commit the `.ddev/.env.opencode` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `OPENCODE_DOCKER_IMAGE` | `--opencode-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@dragonwize](https://github.com/dragonwize)**
