# Security Policy

## 🛡️ Supported Versions

We actively support and provide security updates for the following versions:

| Version | Supported          |
| ------- | ------------------ |
| 1.x.x   | ✅ Active support  |
| 0.9.x   | ⚠️ Limited support |
| < 0.9   | ❌ No longer supported |

## 🔒 Security Considerations

### What We Protect
- **Installation integrity** - Ensuring downloaded PowerToys binaries are authentic
- **System security** - Preventing privilege escalation or unauthorized access
- **User privacy** - No data collection or tracking during installation
- **Network security** - Safe handling of downloads and verification

### What We Don't Handle
- **Microsoft PowerToys vulnerabilities** - Report directly to Microsoft
- **Windows OS security issues** - Report to Microsoft Security Response Center
- **Third-party tools** - Report to respective maintainers

## 🚨 Reporting a Vulnerability

### For Critical Security Issues
**Please DO NOT open public issues for security vulnerabilities.**

Instead, report security issues privately:

1. **Email**: Send details to `security@microsofttoois.github.io`
2. **Subject**: `[SECURITY] Brief description of the issue`
3. **Content**: Include detailed reproduction steps and impact assessment

### For Non-Critical Security Concerns
You can open a public issue for:
- General security best practices
- Documentation improvements
- Configuration recommendations
- Non-sensitive hardening suggestions

## 📋 Vulnerability Report Template

Please include the following information:

### Basic Information
- **Type**: What kind of vulnerability (e.g., code injection, privilege escalation)
- **Component**: Which part of the installer is affected
- **Severity**: Your assessment of the impact (Low/Medium/High/Critical)

### Environment Details
- **Windows Version**: (e.g., Windows 11 22H2)
- **PowerToys Version**: Which version were you trying to install
- **Tool Version**: Version of our installer that has the vulnerability
- **User Context**: Standard user or administrator

### Reproduction Steps
1. Detailed step-by-step instructions
2. Any specific conditions required
3. Expected vs. actual behavior
4. Screenshots or logs (if safe to share)

### Impact Assessment
- Who could be affected?
- What could an attacker achieve?
- Are there any mitigating factors?
- Suggested remediation steps

## ⏱️ Response Timeline

### Initial Response
- **Critical vulnerabilities**: Within 24 hours
- **High severity**: Within 48 hours  
- **Medium/Low severity**: Within 1 week

### Resolution Timeline
- **Critical**: Emergency fix within 72 hours
- **High**: Patch within 2 weeks
- **Medium**: Fix in next regular release
- **Low**: Address in future release

## 🔐 Security Best Practices

### For Users
- **Always run as administrator** - Our installer requires elevated privileges
- **Download from official sources** - Only use releases from this repository
- **Verify checksums** - Check file integrity before installation
- **Keep Windows updated** - Ensure your system has latest security patches
- **Use antivirus software** - Scan downloads with updated antivirus

### For Contributors
- **Code review required** - All security-related changes need review
- **Input validation** - Always validate user inputs and file paths
- **Principle of least privilege** - Request minimal necessary permissions
- **Secure defaults** - Default configurations should be secure
- **Error handling** - Don't expose sensitive information in error messages

## 🛠️ Security Features

### Built-in Protections
- ✅ **Digital signature verification** - Validates PowerToys installer authenticity
- ✅ **Checksum validation** - Ensures file integrity during download
- ✅ **Safe file handling** - Prevents path traversal and injection attacks
- ✅ **Privilege validation** - Confirms administrative rights before execution
- ✅ **Error isolation** - Prevents information disclosure through error messages

### Download Security
- All PowerToys binaries are downloaded from official Microsoft sources
- SHA256 checksums verified for all downloaded files
- TLS/HTTPS enforced for all network communications
- No third-party or unofficial download sources

### Installation Security
- Temporary files cleaned up after installation
- Registry changes made safely with proper validation
- Service installation follows Windows security guidelines
- No modifications to critical system files

## 🚫 Known Security Limitations

### By Design
- **Requires administrator privileges** - Necessary for system-level installation
- **Downloads from internet** - Required to get latest PowerToys binaries
- **Modifies system registry** - Needed for proper PowerToys integration
- **Installs system services** - Required for PowerToys functionality

### Mitigations
- All operations clearly documented and transparent
- User consent required for each major step
- Rollback capabilities for most operations
- Detailed logging for audit purposes

## 🔍 Security Auditing

### Self-Assessment
We regularly review our codebase for:
- Input validation vulnerabilities
- Privilege escalation risks
- Information disclosure issues
- Download and installation security

### External Review
We welcome security researchers to:
- Review our source code
- Test our installation process
- Suggest security improvements
- Report potential vulnerabilities

### Bounty Program
Currently, we don't offer a formal bug bounty program, but we:
- Acknowledge security researchers in our README
- Provide recognition for significant discoveries
- Consider featuring major contributors

## 📝 Security Updates

### Communication
- Security fixes are clearly marked in release notes
- Critical vulnerabilities get dedicated security advisories
- Users notified through GitHub releases and discussions

### Update Process
- Critical fixes released as emergency patches
- Regular security updates included in normal releases
- Clear upgrade instructions provided for all security updates

## ⚖️ Legal and Compliance

### Responsible Disclosure
We follow responsible disclosure practices:
- Work with reporters to understand and fix issues
- Coordinate public disclosure timing
- Credit researchers appropriately
- Share technical details after fixes are available

### Privacy
- No personal information collected during installation
- No analytics or telemetry data sent
- Local logs contain only technical debugging information
- Users have full control over all data

## 📞 Contact Information

### Security Team
- **Primary**: `security@microsofttoois.github.io`
- **Backup**: Open a private GitHub discussion

### General Support
- **Issues**: Use GitHub Issues for non-security bugs
- **Discussions**: Use GitHub Discussions for questions
- **Documentation**: Check our comprehensive README first

---

**Thank you for helping keep our community safe! 🔒** 