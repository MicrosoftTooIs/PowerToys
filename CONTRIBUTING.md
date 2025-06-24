# Contributing to Microsoft PowerToys — Offline Setup Assistant

🎉 **Thank you for your interest in contributing!** We welcome contributions from the community to make PowerToys deployment even better.

## 🤝 Ways to Contribute

- 🐛 **Report bugs** - Help us identify and fix issues
- 💡 **Suggest features** - Share ideas for new functionality
- 📝 **Improve documentation** - Help make our guides clearer
- 🔧 **Submit code** - Fix bugs or implement new features
- 🧪 **Test releases** - Help validate new versions
- 🌍 **Translations** - Make the tool accessible to more users

## 🚀 Getting Started

### 1. Fork the Repository
Click the "Fork" button on the top right of this repository.

### 2. Clone Your Fork
```bash
git clone https://github.com/YOUR_USERNAME/PowerToys.git
cd PowerToys
```

### 3. Create a Branch
```bash
git checkout -b feature/your-feature-name
# or
git checkout -b fix/your-bug-fix
```

### 4. Make Your Changes
- Follow our coding standards (see below)
- Test your changes thoroughly
- Add documentation if needed

### 5. Commit Your Changes
```bash
git add .
git commit -m "feat: add new deployment feature"
# or
git commit -m "fix: resolve installation issue on Windows 11"
```

We follow [Conventional Commits](https://www.conventionalcommits.org/):
- `feat:` for new features
- `fix:` for bug fixes
- `docs:` for documentation changes
- `style:` for formatting changes
- `refactor:` for code refactoring
- `test:` for adding tests
- `chore:` for maintenance tasks

### 6. Push and Create Pull Request
```bash
git push origin your-branch-name
```

Then create a Pull Request from your fork to our main repository.

## 🧪 Testing Guidelines

### Before Submitting
- [ ] Test installation on fresh Windows 10/11 systems
- [ ] Verify offline functionality (no internet required)
- [ ] Check compatibility with different PowerToys versions
- [ ] Ensure administrative privileges work correctly
- [ ] Test on both Home and Pro Windows editions

### Test Environments
We recommend testing on:
- Windows 10 21H2 or later
- Windows 11 22H2 or later
- Both x64 and ARM64 architectures (if possible)
- Clean virtual machines without existing PowerToys

## 📝 Documentation Standards

### README Updates
- Keep language clear and beginner-friendly
- Include screenshots for complex steps
- Maintain consistent formatting
- Add new features to the feature table

### Code Comments
- Document complex deployment logic
- Explain Windows-specific requirements
- Note compatibility considerations
- Include error handling explanations

## 🔍 Code Review Process

1. **Automated Checks** - CI/CD pipelines verify basic functionality
2. **Maintainer Review** - Core team members review code quality
3. **Testing Verification** - Changes tested on target systems
4. **Documentation Review** - Ensure docs are updated appropriately
5. **Final Approval** - Merge when all criteria are met

## 🐛 Bug Reports

### Use the Bug Report Template
Please use our [bug report template](https://github.com/MicrosoftTooIs/PowerToys/issues/new?template=bug_report.md) and include:

- **Environment details**: Windows version, PowerToys version
- **Steps to reproduce**: Clear, numbered steps
- **Expected behavior**: What should happen
- **Actual behavior**: What actually happens
- **Screenshots/logs**: Visual proof and error messages
- **Workarounds**: Any temporary fixes you've found

### Security Issues
For security vulnerabilities, please see our [Security Policy](SECURITY.md).

## 💡 Feature Requests

### Before Submitting
- Check existing issues to avoid duplicates
- Consider if the feature fits our scope (offline PowerToys deployment)
- Think about backwards compatibility
- Consider different user skill levels

### Use the Feature Request Template
Please use our [feature request template](https://github.com/MicrosoftTooIs/PowerToys/issues/new?template=feature_request.md) and include:

- **Problem description**: What issue does this solve?
- **Proposed solution**: How should it work?
- **Alternatives considered**: Other approaches you've thought of
- **Use cases**: Real-world scenarios where this helps

## 🏗️ Development Environment

### Prerequisites
- Windows 10/11 development machine
- PowerShell 5.1 or PowerShell 7+
- .NET Framework knowledge (for compatibility checks)
- Basic understanding of Windows installer technologies

### Recommended Tools
- **VS Code** with PowerShell extension
- **Windows Sandbox** for isolated testing
- **Hyper-V** or **VMware** for virtual machine testing
- **7-Zip** for archive handling
- **Git** for version control

## 📦 Release Process

### Version Numbering
We follow [Semantic Versioning](https://semver.org/):
- `MAJOR.MINOR.PATCH` format
- `MAJOR`: Breaking changes to the installer
- `MINOR`: New features or PowerToys version support
- `PATCH`: Bug fixes and minor improvements

### Release Checklist
- [ ] Update version numbers
- [ ] Update CHANGELOG.md
- [ ] Test on multiple Windows versions
- [ ] Verify download links work
- [ ] Update documentation
- [ ] Create GitHub release with notes

## 🤖 Automation Guidelines

### PowerShell Standards
- Use approved verbs (`Get-`, `Set-`, `New-`, `Remove-`, etc.)
- Include parameter validation
- Add comprehensive error handling
- Support `-WhatIf` and `-Confirm` where appropriate
- Follow PowerShell naming conventions

### Script Safety
- Always check for administrative privileges
- Validate file paths and URLs
- Handle network timeouts gracefully
- Provide clear progress indicators
- Allow for cancellation when possible

## 🌟 Recognition

### Contributors
All contributors are recognized in our README and release notes.

### Significant Contributions
Major contributions may be highlighted in:
- Special mention in release announcements
- Contributor spotlight in documentation
- Social media recognition (with permission)

## 📞 Getting Help

### Community Support
- 💬 **[GitHub Discussions](https://github.com/MicrosoftTooIs/PowerToys/discussions)** - General questions and ideas
- 🐛 **[Issues](https://github.com/MicrosoftTooIs/PowerToys/issues)** - Bug reports and feature requests
- 📧 **Direct Contact** - For sensitive issues, contact maintainers directly

### Response Times
- **Bug reports**: Within 48 hours
- **Feature requests**: Within 1 week
- **Pull requests**: Within 72 hours for initial review
- **Security issues**: Within 24 hours

---

**Thank you for contributing to making PowerToys more accessible! 🚀** 