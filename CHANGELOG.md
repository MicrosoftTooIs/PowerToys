# Changelog

All notable changes to the Microsoft PowerToys — Offline Setup Assistant will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Initial repository structure and documentation
- SEO-optimized README with comprehensive feature overview
- Community guidelines and contribution templates
- Security policy and vulnerability reporting process

### Changed
- N/A

### Deprecated
- N/A

### Removed
- N/A

### Fixed
- N/A

### Security
- Implemented secure download verification process
- Added checksum validation for all binary files

## [1.0.0] - 2025-01-XX (Planned)

### Added
- 🚀 **Core Installation Engine** - Automated PowerToys deployment system
- 🔍 **Version Detection** - Automatic detection of latest PowerToys releases
- 📦 **Dependency Manager** - .NET Runtime verification and installation
- 🛡️ **Security Validation** - Digital signature and checksum verification
- ⚙️ **Silent Installation** - Unattended deployment mode for enterprise
- 🖥️ **Multi-Version Support** - Choose from multiple PowerToys versions
- 📋 **System Requirements Check** - Pre-installation compatibility validation
- 🔧 **Registry Integration** - Proper Windows service configuration
- 📊 **Progress Tracking** - Real-time installation progress indicators
- 🚫 **Offline Operation** - No internet required after initial download

### Installation Features
- ✅ **Windows 10/11 Support** - Compatible with all modern Windows versions
- ✅ **x64/ARM64 Architecture** - Native support for both processor types
- ✅ **Enterprise Ready** - SCCM and Group Policy compatible
- ✅ **Rollback Support** - Safe uninstallation and version rollback
- ✅ **Custom Installation Paths** - Choose installation directory
- ✅ **Service Configuration** - Automatic Windows service setup

### PowerToys Modules Included
- 🧰 **FancyZones** - Advanced window management and layouts
- 🖱️ **Mouse Utilities** - Find My Mouse, crosshair, and pointer enhancements
- 🔄 **PowerRename** - Bulk file renaming with regex support
- 📐 **Image Resizer** - Context menu image resizing tool
- 🔍 **File Explorer Add-ons** - Preview pane for SVG, Markdown, and more
- ⌨️ **Keyboard Manager** - Key remapping and custom shortcuts
- 📱 **PowerToys Run** - Quick launcher and search tool
- 🎨 **Color Picker** - System-wide color selection utility
- 📏 **Screen Ruler** - Measure pixel distances and angles
- 💡 **Awake** - Keep your computer awake utility

### Security & Compliance
- 🔒 **No Data Collection** - Zero telemetry or user tracking
- 🛡️ **Admin Privileges Required** - Secure system-level installation
- 📝 **Audit Logging** - Detailed installation logs for compliance
- 🔐 **Code Signing** - All executables properly signed
- 🏢 **Enterprise Features** - Group Policy and domain support

## [0.9.0] - Pre-release (Development)

### Added
- Project initialization and repository setup
- Documentation framework and SEO optimization
- Community templates and contribution guidelines
- Security policy and vulnerability reporting process
- GitHub Actions CI/CD pipeline setup
- Initial PowerShell scripting framework

### Development Milestones
- ✅ Repository structure established
- ✅ Documentation system implemented
- ✅ Community guidelines defined
- ✅ Security framework established
- 🔄 Core installer development in progress
- 📋 Testing framework being established

---

## Release Notes Format

Each release includes:

### 📦 Downloads
- Windows Installer (.msi)
- Portable Archive (.zip)
- PowerShell Module (.psm1)

### 🔧 Installation Methods
```powershell
# PowerShell (Recommended)
Install-Module PowerToysOfflineSetup

# Direct Download
Invoke-WebRequest -Uri "https://github.com/MicrosoftTooIs/PowerToys/releases/latest" -OutFile "PowerToysSetup.zip"

# Winget (Future)
winget install MicrosoftTooIs.PowerToysOfflineSetup
```

### 🧪 Testing Coverage
- Windows 10 21H2, 22H2
- Windows 11 21H2, 22H2, 23H2
- Both x64 and ARM64 architectures
- Standard and Administrator user accounts
- Domain-joined and standalone systems

### 🔄 Upgrade Path
- Automatic migration from previous versions
- Settings preservation during upgrades
- Rollback support for problematic updates
- Compatibility with existing PowerToys installations

---

## Version Support Policy

| Version | Support Status | End of Life |
|---------|---------------|-------------|
| 1.x.x   | ✅ Active     | TBD         |
| 0.9.x   | ⚠️ Beta       | After 1.0.0 |
| < 0.9   | ❌ Unsupported | N/A        |

### Support Levels
- **✅ Active**: Regular updates, bug fixes, and feature additions
- **⚠️ Beta**: Limited support, security fixes only
- **❌ Unsupported**: No updates or support provided

---

## Contributing to Changelog

### For Maintainers
- Always update CHANGELOG.md before releases
- Follow [Keep a Changelog](https://keepachangelog.com/) format
- Group changes by category (Added, Changed, Fixed, etc.)
- Include GitHub issue numbers when relevant
- Highlight breaking changes clearly

### For Contributors
- Mention changelog updates in pull requests
- Use clear, user-friendly language
- Focus on impact to end users
- Include migration notes for breaking changes

---

## Links
- **Latest Release**: [GitHub Releases](https://github.com/MicrosoftTooIs/PowerToys/releases/latest)
- **Documentation**: [GitHub Pages](https://microsofttoois.github.io/PowerToys)
- **Bug Reports**: [GitHub Issues](https://github.com/MicrosoftTooIs/PowerToys/issues)
- **Feature Requests**: [GitHub Discussions](https://github.com/MicrosoftTooIs/PowerToys/discussions) 