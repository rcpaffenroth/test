# test

## UV notes

This is a test repository for UV. It contains a simple `pyproject.toml` file and a `README.md` file. The `pyproject.toml` file specifies the project metadata, dependencies, and pytest configuration. The `README.md` file provides a brief description of the project.

```bash
# To install the dependencies, run:
uv sync 
# To run the tests, run:
uv run pytest
```

```bash
# To generate requirements.txt, run:
uv export -o requirements.txt 
```

```bash
# Can be installed using pip, but it's recommended to use UV for managing dependencies and running tests:
pip install -r requirements.txt
```

