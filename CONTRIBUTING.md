# Contributing to teste123

Thank you for your interest in contributing to this project! This document provides guidelines for contributing using GitFlow methodology.

## GitFlow Workflow

We use GitFlow for our branching strategy. Please familiarize yourself with the workflow:

### Branch Types

- **main**: Production-ready code
- **develop**: Integration branch for features
- **feature/**: New feature development
- **release/**: Release preparation
- **hotfix/**: Critical production fixes

### Development Process

1. **Feature Development**
   ```bash
   git checkout develop
   git pull origin develop
   git checkout -b feature/your-feature-name
   # Make your changes
   git commit -m "feat: add new feature"
   git push origin feature/your-feature-name
   # Create PR to develop branch
   ```

2. **Bug Fixes**
   ```bash
   git checkout develop
   git pull origin develop
   git checkout -b feature/fix-issue-name
   # Fix the issue
   git commit -m "fix: resolve issue description"
   git push origin feature/fix-issue-name
   # Create PR to develop branch
   ```

3. **Hotfixes**
   ```bash
   git checkout main
   git pull origin main
   git checkout -b hotfix/critical-fix
   # Apply critical fix
   git commit -m "fix: critical security issue"
   git push origin hotfix/critical-fix
   # Create PR to main AND develop branches
   ```

## Code Standards

- Write clear, descriptive commit messages
- Follow existing code style and conventions
- Add tests for new features
- Update documentation as needed
- Ensure all CI checks pass

## Pull Request Process

1. Create feature branch from develop
2. Make your changes with clear commits
3. Write/update tests as necessary
4. Update documentation if needed
5. Create pull request with detailed description
6. Address any review feedback
7. Merge will be handled by maintainers

## Getting Help

- Check existing issues and discussions
- Create new issue for bugs or feature requests
- Contact maintainers for urgent matters

Thank you for contributing!
