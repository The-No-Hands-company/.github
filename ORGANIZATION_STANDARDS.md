# The No Hands Company - Organization Standards

This document outlines the standards and best practices for repositories within The No Hands Company GitHub organization.

## Repository Naming Conventions

- Use PascalCase for all repository names (e.g., `VersaEngine`, `VersaUI`)
- Use descriptive names that clearly indicate the repository's purpose
- Avoid abbreviations unless they are widely understood

## Repository Structure

All repositories should follow this general structure:

```
Repository/
├── .github/                    # GitHub specific files
│   ├── workflows/              # GitHub Actions workflows
│   └── ISSUE_TEMPLATE/         # Issue templates
├── docs/                       # Documentation
├── src/ or lib/                # Source code
├── tests/                      # Tests
├── examples/                   # Example code
├── .gitignore                  # Git ignore file
├── LICENSE                     # License file
├── README.md                   # Repository README
└── CONTRIBUTING.md             # Contribution guidelines
```

## Branch Naming Conventions

- `main` - Main development branch
- `feature/feature-name` - Feature branches
- `bugfix/issue-description` - Bug fix branches
- `hotfix/issue-description` - Critical fixes
- `release/vX.Y.Z` - Release branches

## Commit Message Guidelines

Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

Types:
- `feat:` - A new feature
- `fix:` - A bug fix
- `docs:` - Documentation changes
- `style:` - Code style changes (formatting, etc.)
- `refactor:` - Code changes that neither fix bugs nor add features
- `perf:` - Performance improvements
- `test:` - Adding or correcting tests
- `chore:` - Changes to the build process or auxiliary tools

## Pull Request Process

1. Create a branch following naming conventions
2. Make your changes
3. Write or update tests as needed
4. Ensure all tests pass
5. Submit a pull request to the `main` branch
6. Fill out the pull request template
7. Wait for review
8. Address feedback

## Code Style Guidelines

### C++
- Follow C++17 standard
- Use [clang-format](https://clang.llvm.org/docs/ClangFormat.html) with our style configuration
- Follow the [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html) with our modifications

### JavaScript/TypeScript
- Use [ESLint](https://eslint.org/) with our configuration
- Use [Prettier](https://prettier.io/) for formatting
- Follow [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)

## Documentation Requirements

All repositories must include:
- A README.md with:
  - Project description
  - Features
  - Installation instructions
  - Usage examples
  - License information
- API documentation
- Contributing guidelines
- Code comments explaining complex logic

## Testing Standards

- All code should have appropriate unit tests
- Integration tests should be included for API endpoints and complex features
- Aim for >80% code coverage
- All tests must pass before merging

## Security Guidelines

- Follow the principle of least privilege
- Never commit sensitive information (API keys, passwords, etc.)
- Keep dependencies updated
- Use security scanning tools
- Follow the security policy defined in SECURITY.md

## Using Templates

The organization provides several templates to ensure consistency:

1. **Workflow Templates**
   - Located in `.github/workflow-templates/`
   - Use these as starting points for your GitHub Actions workflows

2. **Project Templates**
   - Located in `.github/project-templates/`
   - Use these to create new repositories with consistent structure

## License

All projects should use the MIT License unless there's a specific reason to use a different license.

## Questions?

For questions about these standards, please contact the organization admins. 