# Copier UV Template

This is a very simple [copier](https://github.com/copier-org/copier) template for Python projects with src layout and dependency management by [uv](https://github.com/astral-sh/uv).

## Features

- Automated copier questions
- Setup for [uv](https://github.com/astral-sh/uv)
- Included dev tools for formatting, quality checks and testing: 
    - [ruff](https://github.com/astral-sh/ruff) 
    - [pre-commit](https://github.com/pre-commit/pre-commit)
    - [black](https://github.com/psf/black)
    - [pytest](https://github.com/pytest-dev/pytest/)
- The project is structured in the [src layout](https://www.pyopensci.org/python-package-guide/package-structure-code/python-package-structure.html)

##  Usage
### Requirements
You need to have uv and copier installed. Install uv and an accompanying Python version (or use your own Python environment like pyenv or conda):
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
# optional:
uv python install 3.12
```

Install copier with uv or pipx (this will install uv globally):
```bash
pipx install copier
```
or
```bash
uv tool install copier
```

### Generate a Project
To generate a new project, execute the following command:
```bash
copier copy --trust "gh:jkoessle/uv-copier-template" /path/to/your/new/project
```

It's also possible to use uv directly, without the need to install copier:
```bash
uvx copier copy --trust "gh:jkoessle/uv-copier-template" /path/to/your/new/project
```
