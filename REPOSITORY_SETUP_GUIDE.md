# The No Hands Company - Repository Setup Guide

This guide walks you through setting up a new repository within The No Hands Company GitHub organization.

## Step 1: Create a New Repository

1. Go to [The No Hands Company GitHub Organization](https://github.com/The-No-Hands-company)
2. Click on "New Repository"
3. Name your repository following our naming conventions (PascalCase)
4. Add a brief description
5. Select "Private" (we'll make it public later if needed)
6. Select "Add a README file"
7. Select "Add .gitignore" (choose the appropriate template)
8. Select "Choose a license" (MIT License recommended)
9. Click "Create repository"

## Step 2: Clone the Repository Locally

```bash
git clone https://github.com/The-No-Hands-company/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

## Step 3: Set Up Repository Structure

You have two options:

### Option A: Use a Project Template

1. Choose the appropriate template from `.github/project-templates/`
2. Copy the template files to your repository
3. Update files with your project details

### Option B: Manual Setup

1. Create the following directory structure:
   ```
   YOUR_REPO_NAME/
   ├── .github/
   │   ├── workflows/
   │   └── ISSUE_TEMPLATE/
   ├── docs/
   ├── src/ (or lib/)
   ├── tests/
   └── examples/
   ```

2. Copy standard files from the `.github` repository:
   - CONTRIBUTING.md
   - Code of Conduct reference
   - Security policy reference
   - Issue templates

## Step 4: Set Up GitHub Actions

1. Create a GitHub Actions workflow file:
   - For C++ projects, copy from `.github/workflow-templates/cpp-cmake-build.yml`
   - For Node.js projects, copy from `.github/workflow-templates/nodejs-build.yml`
   - For other project types, create a custom workflow

2. Save the workflow file to `.github/workflows/build.yml`

## Step 5: Update Repository Settings

1. Go to your repository's Settings
2. Under "General", enable "Automatically delete head branches"
3. Under "Branches", add a branch protection rule for `main`:
   - Require pull request reviews before merging
   - Require status checks to pass before merging
   - Require linear history
   - Include administrators

## Step 6: Set Up Documentation

1. Create a comprehensive README.md:
   - Project description
   - Features
   - Setup instructions
   - Usage examples
   - Contributing section
   - License information

2. Set up additional documentation in the `docs/` directory:
   - Getting started guide
   - API documentation
   - Development guide

## Step 7: Initial Commit and Push

```bash
git add .
git commit -m "chore: initial repository setup"
git push origin main
```

## Step 8: Set Up Project Board (Optional)

1. Go to the "Projects" tab
2. Click "Create a project"
3. Choose "Board" template
4. Set up columns: Todo, In Progress, Review, Done
5. Add initial issues to the board

## Step 9: Add Repository Topics

1. Go to the repository page
2. Next to "About", click the ⚙️ icon
3. Add relevant topics (e.g., "the-no-hands-company", "cpp", "game-engine", etc.)
4. Update the description and website if available

## Step 10: Final Check

Use this checklist to ensure you've completed all steps:

- [ ] Repository created with correct name
- [ ] Directory structure set up
- [ ] Standard files added (README, LICENSE, etc.)
- [ ] GitHub Actions workflow added
- [ ] Branch protection rules configured
- [ ] Documentation created
- [ ] Project board set up (if needed)
- [ ] Repository topics added

## Need Help?

If you need help with any of these steps, please contact the organization administrators. 