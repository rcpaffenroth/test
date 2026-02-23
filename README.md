# test

A Python project for testing UV package management and pytest notebook integration.

## Features

- Python 3.10+ with modern dependency management via [UV](https://docs.astral.sh/uv/)
- pytest configuration with [nbmake](https://github.com/mariusvniekerk/nbmake) for notebook testing
- Pre-configured dev container for consistent development environment
- CI/CD pipeline for automated testing

## Installation

### Prerequisites

- Python 3.10 or higher
- [UV](https://docs.astral.sh/uv/getting-started/installation/) package manager

### Setup

```bash
# Install all dependencies (including dev tools)
uv sync

# Install only runtime dependencies
uv sync --no-dev
```

## Usage

### Running Tests

```bash
# Run all tests (Python files and Jupyter notebooks)
uv run pytest

# Run with verbose output
uv run pytest -v
```

### Managing Dependencies

```bash
# Add a runtime dependency
uv add <package>

# Add a development dependency
uv add --dev <package>

# Remove a dependency
uv remove <package>

# Export requirements.txt for pip compatibility
uv export -o requirements.txt
```

### Running the Application

```bash
# Run the main script
uv run python main.py
```

## Project Structure

```
test/
├── main.py              # Entry point
├── pyproject.toml       # Project configuration
├── README.md            # This file
├── tests/
│   ├── test_1.py        # Unit tests
│   └── test.ipynb       # Jupyter notebook tests
└── .devcontainer/       # Dev container configuration
```

## Development

### Dev Container

Open this repository in VS Code with the [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) for a pre-configured development environment.

### Dev Container setup

```bash
pipx install uv
uv sync
uv run pytest
```

