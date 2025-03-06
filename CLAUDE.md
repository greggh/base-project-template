# Project: Base Project Template

## Overview
Base Project Template serves as the foundation template for all new projects in the Neovim ecosystem. It provides standardized GitHub configurations, workflow templates, documentation structures, and development best practices that form the base layer for more specialized project templates.

## Essential Commands
- Check Documentation: `env -C /home/gregg/Projects/base-project-repo markdownlint *.md`
- Fix Documentation: `env -C /home/gregg/Projects/base-project-repo markdownlint --fix *.md`
- Version Check: `env -C /home/gregg/Projects/base-project-repo lua scripts/version_check.lua`
- Version Bump: `env -C /home/gregg/Projects/base-project-repo lua scripts/version_bump.lua patch`
- Setup Hooks: `env -C /home/gregg/Projects/base-project-repo ./scripts/setup-hooks.sh`

## Project Structure
- `/.github`: GitHub workflows and templates
- `/docs`: Documentation structure
- `/scripts`: Utility scripts for development
- `/.githooks`: Git hooks for pre-commit validation
- `/templates`: Template files for various purposes
- `CHANGELOG.md`, `README.md`, etc.: Standard documentation files

## Current Focus
- Fixing remaining YAML linting issues in workflow files
- Creating standardized workflow file templates
- Adding hooks-util as git submodule
- Improving documentation structure and style
- Enhancing version management scripts

## Documentation Links
- Tasks: `/home/gregg/Projects/docs-projects/neovim-ecosystem-docs/tasks/base-project-tasks.md`
- Project Status: `/home/gregg/Projects/docs-projects/neovim-ecosystem-docs/project-status.md`