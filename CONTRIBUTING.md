# Contributing to Secure Medical Data Sharing System

First off, thank you for considering contributing to this project! It's people like you that make this educational tool better for everyone.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Pull Request Process](#pull-request-process)
- [Coding Standards](#coding-standards)
- [Commit Message Guidelines](#commit-message-guidelines)

## Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to the project maintainers.

### Our Standards

- Using welcoming and inclusive language
- Being respectful of differing viewpoints and experiences
- Gracefully accepting constructive criticism
- Focusing on what is best for the community
- Showing empathy towards other community members

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the existing issues to avoid duplicates. When you create a bug report, include as many details as possible:

- **Use a clear and descriptive title**
- **Describe the exact steps to reproduce the problem**
- **Provide specific examples**
- **Describe the behavior you observed and what you expected**
- **Include screenshots if possible**
- **Include your environment details** (OS, browser, Node version)

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, include:

- **Use a clear and descriptive title**
- **Provide a detailed description of the suggested enhancement**
- **Explain why this enhancement would be useful**
- **List any similar features in other applications**

### Your First Code Contribution

Unsure where to begin? Look for issues tagged with:
- `good-first-issue` - Good for newcomers
- `help-wanted` - Extra attention needed
- `documentation` - Documentation improvements

## Development Setup

1. Fork the repository
2. Clone your fork:
   ```bash
   git clone https://github.com/your-username/secure-medical-data-sharing.git
   ```

3. Install dependencies:
   ```bash
   cd secure-medical-data-sharing
   npm install
   ```

4. Create a branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```

5. Make your changes and test thoroughly

6. Run the application:
   ```bash
   npm start
   ```

## Pull Request Process

1. **Update documentation** - Ensure the README.md and other docs reflect your changes

2. **Follow coding standards** - Make sure your code follows the project's style guidelines

3. **Write meaningful commit messages** - Follow the commit message guidelines below

4. **Test your changes** - Ensure everything works as expected

5. **Update the CHANGELOG** - Add a note about your changes

6. **Submit the PR** with a clear title and description:
   - Reference any related issues
   - Describe what changes you made and why
   - Include screenshots for UI changes

7. **Wait for review** - Maintainers will review your PR and may request changes

8. **Address feedback** - Make requested changes and push to your branch

## Coding Standards

### JavaScript/React

- Use functional components with hooks
- Follow ESLint rules (if configured)
- Use meaningful variable and function names
- Add comments for complex logic
- Keep components small and focused
- Use proper PropTypes or TypeScript (if applicable)

### Code Style

```javascript
// Good
const handleEncrypt = () => {
  if (!selectedUser || !medicalData) {
    addLog('ERROR: Please select a user and enter medical data');
    return;
  }
  // ... rest of the function
};

// Bad
function encrypt(){
if(!user||!data)return
// ...
}
```

### File Organization

- Keep related functionality together
- Use clear, descriptive file names
- Follow the existing project structure
- Don't create unnecessary files or folders

## Commit Message Guidelines

### Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- **feat**: New feature
- **fix**: Bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting, missing semicolons, etc.)
- **refactor**: Code refactoring
- **test**: Adding or updating tests
- **chore**: Maintenance tasks

### Examples

```
feat(encryption): add RSA encryption support

Implemented RSA-2048 encryption as an alternative to XOR cipher
for improved security in production environments.

Closes #123
```

```
fix(ui): correct button alignment on mobile devices

Buttons were overlapping on screens smaller than 768px.
Added responsive classes to fix the layout.
```

```
docs(readme): update installation instructions

Added troubleshooting section for common npm install errors.
```

## Testing Guidelines

- Test all new features manually
- Test on different browsers (Chrome, Firefox, Safari)
- Test responsive design on different screen sizes
- Verify that existing functionality still works
- Test edge cases and error handling

## Questions?

Feel free to open an issue with the `question` label if you have any questions about contributing.

## Recognition

Contributors will be recognized in the project README. Thank you for your contribution!

