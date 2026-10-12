# Contributing to My Agent Demo

Thank you for considering contributing to **My Agent Demo**! We appreciate your help in making this project better. Please follow the guidelines below to ensure a smooth contribution process.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Submitting Pull Requests](#submitting-pull-requests)
- [Development Setup](#development-setup)
- [Coding Standards](#coding-standards)
- [Testing](#testing)
- [Commit Message Guidelines](#commit-message-guidelines)
- [License](#license)

## Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct. By participating, you are expected to uphold this code. Please read the full [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for details.

## How to Contribute

### Reporting Bugs

1. **Search existing issues** to see if the bug has already been reported.
2. If not, open a new issue with:
   - A clear title.
   - Steps to reproduce the bug.
   - Expected vs. actual behavior.
   - Any relevant logs or screenshots.

### Suggesting Enhancements

1. Check the issue tracker for similar feature requests.
2. If none exist, open a new issue describing the enhancement, including:
   - Motivation and use‑case.
   - Proposed implementation details.
   - Potential impact on existing functionality.

### Submitting Pull Requests

1. **Fork the repository** and create a new branch for your work:
   ```bash
   git checkout -b my-feature-branch
   ```
2. **Make your changes**, ensuring they adhere to the coding standards (see below).
3. **Write tests** for new functionality or bug fixes.
4. **Run the test suite** to ensure everything passes:
   ```bash
   pytest
   ```
5. **Commit your changes** with a clear, descriptive commit message (see guidelines).
6. **Push** your branch to your fork and open a pull request against the `main` branch.
7. Fill out the PR template, linking any related issues.

## Development Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/my-agent-demo.git
   cd my-agent-demo
   ```
2. **Create a virtual environment** (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # Windows: venv\Scripts\activate
   ```
3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
4. **Set your OpenAI API key** as an environment variable:
   ```bash
   export OPENAI_API_KEY='your-api-key'
   ```

## Coding Standards

- Follow **PEP 8** style guidelines.
- Use **type hints** for public functions and methods.
- Keep line length to **79 characters** where possible.
- Write **docstrings** for modules, classes, and public functions using the Google style.
- Prefer **f‑strings** over concatenation for readability.

## Testing

- All new code must include **unit tests** using **pytest**.
- Place tests in the `tests/` directory mirroring the source layout.
- Run the full test suite before submitting a PR:
  ```bash
  pytest
  ```
- Aim for **>90% coverage**; you can check coverage with:
  ```bash
  pytest --cov=.
  ```

## Commit Message Guidelines

Use the **Conventional Commits** format:

```
<type>(<scope>): <subject>

<body>

<footer>
```

- **type**: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`
- **scope** (optional): the part of the codebase affected, e.g., `agent`, `tool`
- **subject**: concise description, max 50 characters.
- **body** (optional): detailed explanation, why the change was needed.
- **footer** (optional): references to issues, e.g., `Closes #123`.

Example:
```
feat(agent): add streaming response support

Implemented a new streaming mode for the OpenAI API wrapper, allowing partial
responses to be processed in real time.

Closes #42
```

## License

By contributing, you agree that your contributions will be licensed under the same MIT License as the project.

---

Thank you for contributing!