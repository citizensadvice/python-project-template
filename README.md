# Python Project Template

A template for Python projects at Citizens Advice.

## What this template includes

- **Project Structure**: A standardized directory layout for Python projects.
- **Dependency Management**: Uses `uv` for managing dependencies and virtual environments.
- **Code Quality**: Pre-configured `ruff` and `ty` set up for code linting, formatting and type-checking.
- **Task Automation**: A `Justfile` for automating common tasks like testing, linting, and formatting.
- **Pre-commit Hooks**: Configured pre-commit hooks for code quality checks (Individual contributors can use `pre-commit` or `prek` for local execution).
- **Code Ownership**: A `CODEOWNERS` file to define code ownership for the repository.
- **Github Actions**: Pre-configured CI workflows for linting.
- **System Packages**: Brewfile for system package installation.

## Project Setup

When starting a new Python project, you can use this template to ensure consistency across projects. Follow these steps to configure this for your own needs:

1. Rename the `python_project_template` directory to your desired project name.
2. Update the `pyproject.toml` file with your project's metadata.
3. Update the `CODEOWNERS` file to reflect the appropriate code owners for your project.
4. Add any additional dependencies to the `pyproject.toml` file as needed.
   - Remember to add dev dependencies to the correct section using `uv add <package> --dev`.
5. Run `just setup` to install dependencies and set up pre-commit hooks.
6. Update the `Justfile` with any custom commands specific to your project.
7. Rewrite the `README.md` file to provide relevant information about your project.
