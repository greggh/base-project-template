# Base Project Template Guide

## Version Management System

### Useful Commands
- Check version consistency: `lua scripts/version_check.lua`
- Bump version: `lua scripts/version_bump.lua 1.2.3`
- Install git hooks: `./scripts/install_hooks.sh`

### Key Files
- `lua/project-name/version.lua` - Single source of truth for version
- `scripts/version_check.lua` - Verifies version consistency across files
- `scripts/version_bump.lua` - Updates version across all project files
- `.githooks/pre-commit` - Git hook for version validation
- `templates/version.lua` - Template for the version file

### Versioning Process
1. Ensure all changes are in the `## [Unreleased]` section of CHANGELOG.md
2. Run version bump script: `lua scripts/version_bump.lua NEW_VERSION`
3. Review changes, especially in CHANGELOG.md
4. Commit with message: `git commit -m "Release: Version NEW_VERSION"`
5. Create a tag: `git tag -a vNEW_VERSION -m "Version NEW_VERSION"`
6. Push changes: `git push && git push --tags`

## Project Setup

### Initial Setup Commands
- Run setup script: `./scripts/setup.sh`
- Apply git hooks: `./scripts/install_hooks.sh`

### Project Files
- `README.md` - Main project documentation
- `CHANGELOG.md` - Project history following Keep a Changelog format
- `CONTRIBUTING.md` - Guidelines for contributors including versioning
- `CODE_OF_CONDUCT.md` - Project code of conduct
- `LICENSE` - Project license
- `SECURITY.md` - Security policy
- `SUPPORT.md` - How to get support

### GitHub Configuration
- `.github/workflows/` - CI, Documentation, and Release workflows
- `.github/ISSUE_TEMPLATE/` - Templates for bug reports and feature requests
- `.github/PULL_REQUEST_TEMPLATE.md` - Template for pull requests