# Contributing Guidelines

Thank you for considering contributing to this project! We welcome contributions from everyone, whether you're fixing a typo, adding new features, or improving documentation.

## Code of Conduct

This project follows our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [maintainer-email].

## Getting Started

1. Fork the repository
2. Clone your fork and create a new branch:
   ```bash
   git clone https://github.com/username/project-name.git
   cd project-name
   git checkout -b my-feature-branch
   ```
3. Set up your development environment following the instructions in [DEVELOPMENT.md](DEVELOPMENT.md)
4. Make your changes
5. Test your changes
6. Push to your fork and submit a pull request

## Development Process

Please see [DEVELOPMENT.md](DEVELOPMENT.md) for details on setting up your development environment and the development workflow.

## Pull Request Process

1. Update the README.md or relevant documentation with details of changes
2. Update the CHANGELOG.md with your changes under the "Unreleased" section
3. Ensure version consistency across the project (see [Versioning](#versioning) below)
4. The PR should work on all supported platforms and pass all tests
5. Your PR needs approval from at least one maintainer before it can be merged

## Versioning

This project follows [Semantic Versioning](https://semver.org/) (MAJOR.MINOR.PATCH).

### Version Management

1. **Single Source of Truth**: The canonical version is stored in `lua/[project-name]/version.lua`.
2. **Consistency**: All references to the version must be consistent across:
   - `README.md`
   - `CHANGELOG.md`
   - Code files (`init.lua`, `main.lua`, etc.)
   - Package files (`.rockspec`, `package.json`, etc.)

### Version Checking

Before committing changes, verify version consistency by running:

```bash
lua scripts/version_check.lua
```

This check is also performed automatically in the pre-commit hook.

### Version Bumping

To update the project version, use the version bump script:

```bash
lua scripts/version_bump.lua NEW_VERSION
```

For example:
```bash
lua scripts/version_bump.lua 1.2.3
```

This will:
1. Update the version in all relevant files
2. Add a new version section to the CHANGELOG.md
3. Update comparison links in the CHANGELOG.md

After running the script, review the changes, commit them, and create a corresponding git tag.

## Coding Standards

- Follow the existing code style and formatting conventions
- Write clear, readable code with helpful comments
- Keep functions small and focused on a single task
- Include appropriate tests for new functionality

## Commit Messages

- Use clear, descriptive commit messages
- Follow the [Conventional Commits](https://www.conventionalcommits.org/) format if possible
- Reference issues and pull requests where appropriate

## License

By contributing to this project, you agree that your contributions will be licensed under the project's license.

## Questions?

If you have any questions, please open an issue or refer to our [SUPPORT.md](SUPPORT.md) file for more information on how to get help.