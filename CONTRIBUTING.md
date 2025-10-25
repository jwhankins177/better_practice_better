# Contributing to Better Practice Bets

Thank you for your interest in contributing! This document provides guidelines for contributing to the project.

## Development Workflow

### Branch Strategy
We use a two-branch workflow:
- **`main`** - Production-ready code, always stable
- **`feature/*`** - Feature branches for new development

### Working on a Feature

1. **Create an Issue First**
   - Go to GitHub Issues
   - Create a new issue describing the feature/bug
   - Wait for discussion/approval if it's a major change

2. **Create a Feature Branch**
   ```bash
   git checkout main
   git pull origin main
   git checkout -b feature/your-feature-name
   ```

3. **Make Your Changes**
   - Write clean, commented code
   - Test thoroughly on multiple devices/browsers
   - Update version number in `index.html`
   - Update `README.md` changelog

4. **Commit Your Changes**
   ```bash
   git add .
   git commit -m "Brief description of changes"
   ```
   
   Use descriptive commit messages:
   - `feat:` for new features
   - `fix:` for bug fixes
   - `improve:` for improvements
   - `docs:` for documentation
   - `style:` for formatting changes

5. **Push and Create Pull Request**
   ```bash
   git push origin feature/your-feature-name
   ```
   - Go to GitHub and create a Pull Request
   - Fill out the PR template completely
   - Link to the related issue

6. **Review Process**
   - PR will be reviewed
   - Address any feedback
   - Once approved, it will be merged to main

### Code Style Guidelines

- Use descriptive variable and function names
- Add comments for complex logic
- Keep functions focused and single-purpose
- Use ES6+ JavaScript features
- Test on both desktop and mobile browsers

### Version Numbers

We use semantic versioning: `MAJOR.MINOR.PATCH`
- **MAJOR**: Breaking changes
- **MINOR**: New features (backward compatible)
- **PATCH**: Bug fixes and small improvements

Update version in:
1. `index.html` (title tag)
2. `index.html` (footer)
3. `README.md` (changelog)

### Testing Checklist

Before submitting a PR, verify:
- [ ] Works on Chrome, Firefox, Safari
- [ ] Works on mobile devices
- [ ] API integration functions correctly
- [ ] Cloud sync works (if applicable)
- [ ] No console errors or warnings
- [ ] Analytics/charts render properly (if applicable)
- [ ] Bankroll calculations are accurate
- [ ] No breaking changes to existing features

### Questions?

Open an issue for questions or clarifications!
