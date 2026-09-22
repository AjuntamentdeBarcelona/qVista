# Contributing to qVista

Thank you for your interest in contributing to **qVista**!

qVista is an open-source Geographic Information System (GIS) application and Python framework developed by the **Ajuntament de Barcelona** (Municipal Institute of Informatics - IMI). We welcome contributions from developers, GIS specialists, and the open-source community.

---

## Code of Conduct

We are committed to providing a welcoming, inclusive, and harassment-free experience for everyone. Please maintain respectful and constructive communication in all project spaces (issues, discussions, and pull requests).

---

## Getting Started

1. **Fork and Clone**:
   Fork the repository on GitHub and clone your fork locally:
   ```bash
   git clone https://github.com/<your-username>/qVista.git
   cd qVista
   ```

2. **Environment Setup**:
   - Install **QGIS 3.10 LTR** or higher (tested on QGIS 3.40 LTR).
   - Verify Python 3 and PyQt5 bindings are properly installed.
   - For configuration profiles, refer to [docs/](docs/).

3. **Coding Standards**:
   - Follow PEP 8 guidelines for Python code.
   - Maintain naming conventions for widgets and classes (e.g. `Qv` prefix for reusable components: `QvCanvas`, `QvLlegenda`, etc.).
   - Refer to [guies/guia-estil.md](guies/guia-estil.md) for detailed coding style patterns.
   - Add docstrings and explanatory comments for public functions and classes.

---

## Submitting Changes

1. **Create a Feature Branch**:
   ```bash
   git checkout -b feature/my-new-feature
   ```

2. **Commit Guidelines**:
   - Write clear, concise commit messages (prefer conventional commit format: `feat:`, `fix:`, `docs:`, `refactor:`).
   - Ensure you do not commit any credentials, tokens, or personal paths.

3. **Open a Pull Request**:
   - Push your branch to your fork.
   - Submit a Pull Request targeting the `main` branch.
   - Describe the changes made, motivation, and any testing performed.

---

## License

By contributing to qVista, you agree that your contributions will be licensed under the project's [GNU General Public License v3.0](LICENSE).
