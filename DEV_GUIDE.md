# Development Quick Reference

## Daily Workflow

### Starting a New Feature
```bash
# 1. Make sure main is up to date
git checkout main
git pull origin main

# 2. Create feature branch
git checkout -b feature/your-feature-name

# 3. Make your changes, test thoroughly

# 4. Commit changes
git add .
git commit -m "feat: description of changes"

# 5. Push branch
git push origin feature/your-feature-name

# 6. Go to GitHub and create Pull Request
```

### Creating an Issue
1. Go to: https://github.com/jwhankins177/better_practice_better/issues
2. Click "New Issue"
3. Choose template (Bug Report, Feature Request, or Improvement)
4. Fill out the template
5. Add labels and milestone

### Branch Naming Convention
- `feature/feature-name` - New features
- `fix/bug-name` - Bug fixes
- `improve/improvement-name` - Improvements to existing features
- `docs/doc-name` - Documentation updates

### Commit Message Format
- `feat:` - New feature
- `fix:` - Bug fix
- `improve:` - Improvement to existing feature
- `docs:` - Documentation changes
- `style:` - Code formatting (no functional changes)
- `refactor:` - Code restructuring (no functional changes)
- `test:` - Adding tests
- `chore:` - Maintenance tasks

### Before Creating a PR
- [ ] Test on desktop browser
- [ ] Test on mobile browser
- [ ] No console errors
- [ ] Version number updated
- [ ] README updated
- [ ] Code is commented
- [ ] Self-reviewed the code

### Current Branches
- `main` - Production (always stable)
- Feature branches are created as needed and deleted after merge

## GitHub URLs
- **Repository**: https://github.com/jwhankins177/better_practice_better
- **Issues**: https://github.com/jwhankins177/better_practice_better/issues
- **Pull Requests**: https://github.com/jwhankins177/better_practice_better/pulls
- **Live App**: https://jwhankins177.github.io/better_practice_better

## Quick Commands
```bash
# Check current branch
git branch

# See uncommitted changes
git status

# See commit history
git log --oneline

# Pull latest from main
git pull origin main

# Delete local branch
git branch -d branch-name

# List all branches (including remote)
git branch -a
```
