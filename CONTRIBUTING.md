# Contributing to MC Mod Updater

Thank you for your interest in contributing to MC Mod Updater! 🎉 We welcome contributions from the community and are grateful for any help to make this tool better for Minecraft players everywhere.

## 📋 Table of Contents

- [Code of Conduct](#-code-of-conduct)
- [Getting Started](#-getting-started)
- [Ways to Contribute](#-ways-to-contribute)
- [Development Setup](#-development-setup)
- [Submitting Changes](#-submitting-changes)
- [Coding Standards](#-coding-standards)
- [Testing Guidelines](#-testing-guidelines)
- [Issue Guidelines](#-issue-guidelines)
- [Pull Request Process](#-pull-request-process)
- [Community and Support](#-community-and-support)

## 🤝 Code of Conduct

This project adheres to a simple code of conduct:
- **Be respectful** and considerate in all interactions
- **Be constructive** with feedback and criticism
- **Focus on the community** and helping Minecraft players
- **Collaborate openly** and share knowledge

We're here to build something awesome together! 🚀

## 🚀 Getting Started

### Prerequisites

Since this is a client-side web application, you only need:
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A text editor or IDE of your choice
- Basic knowledge of HTML, CSS, and JavaScript
- Git for version control

### Quick Start

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/mcmodupdate.app.git
   cd mcmodupdate.app
   ```
3. **Open `index.html`** in your browser or use a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (if you have http-server installed)
   npx http-server
   ```
4. **Make your changes** and test locally
5. **Submit a pull request** when ready!

## 🎯 Ways to Contribute

### 🐛 Bug Reports
Found a bug? Please help us fix it:
- Use our [Bug Report template](https://github.com/mcmodupdate/mcmodupdate.app/issues/new?assignees=&labels=bug%2Cneeds-triage&projects=&template=bug_report.yml)
- Include detailed steps to reproduce
- Provide browser and system information
- Add console errors if available

### ✨ Feature Requests
Have an idea for improvement?
- Use our [Feature Request template](https://github.com/mcmodupdate/mcmodupdate.app/issues/new?assignees=&labels=enhancement%2Cneeds-triage&projects=&template=feature_request.yml)
- Explain the problem your feature solves
- Provide detailed use cases
- Consider how it benefits the broader community

### 💻 Code Contributions
Ready to code? Here's what we need help with:

**High Priority:**
- Performance optimizations
- Mobile UI improvements
- Accessibility enhancements
- Error handling improvements

**Medium Priority:**
- New file format support
- Additional mod platform integrations
- UI/UX enhancements
- Code refactoring and cleanup

**Low Priority:**
- Documentation improvements
- Additional language support
- Advanced features and power-user tools

### 📖 Documentation
Help improve our documentation:
- Fix typos or unclear explanations
- Add examples and use cases
- Improve README sections
- Write tutorials or guides

## 🛠️ Development Setup

### Project Structure
```
mcmodupdate.app/
├── index.html          # Main application file
├── README.md           # Project documentation
├── CONTRIBUTING.md     # This file
├── LICENSE             # MPL-2.0 license
├── netlify.toml        # Deployment configuration
├── site.webmanifest    # PWA manifest
├── sitemap.xml         # SEO sitemap
├── robots.txt          # Search engine directives
├── .github/            # GitHub templates and workflows
│   └── ISSUE_TEMPLATE/ # Issue templates
└── favicon files       # Various favicon formats
```

### Key Technologies
- **Vanilla JavaScript** - No frameworks, maximum performance
- **JSZip** - Reading .jar files and creating .mrpack files
- **TOML.js** - Parsing mod metadata from mods.toml
- **Marked.js** - Rendering markdown changelogs
- **CryptoJS** - SHA-1 hashing for mod identification
- **Modrinth API** - All mod data and version information

### Local Development
1. **Make changes** to `index.html`
2. **Test locally** in multiple browsers
3. **Test with real mod files** to ensure functionality
4. **Check console** for any JavaScript errors
5. **Verify mobile responsiveness** using browser dev tools

## 📝 Submitting Changes

### Before You Start
1. **Check existing issues** to avoid duplicate work
2. **Create an issue** for major changes to discuss approach
3. **Start small** - tackle one feature/bug at a time
4. **Test thoroughly** before submitting

### Making Changes
1. **Create a feature branch** from `main`:
   ```bash
   git checkout -b feature/amazing-feature
   # or
   git checkout -b fix/important-bug
   ```
2. **Make your changes** following our coding standards
3. **Test thoroughly** across different browsers and scenarios
4. **Commit with clear messages**:
   ```bash
   git commit -m "Add feature: bulk mod selection"
   git commit -m "Fix: handle empty mod.toml files gracefully"
   ```

## 🎨 Coding Standards

### HTML
- Use semantic HTML5 elements
- Include proper accessibility attributes
- Maintain clean, readable indentation
- Comment complex sections

### CSS
- Follow the existing CSS custom property patterns
- Use meaningful class names
- Maintain responsive design principles
- Test on mobile devices

### JavaScript
- Use modern ES6+ features where appropriate
- Write clear, self-documenting code
- Add comments for complex logic
- Handle errors gracefully
- Maintain existing code style and patterns

### Performance Considerations
- **Minimize API calls** - Use session caching when possible
- **Handle large files efficiently** - Stream processing for big modpacks
- **Respect rate limits** - Implement proper backoff strategies
- **Optimize for mobile** - Consider bandwidth and processing constraints

## 🧪 Testing Guidelines

### Manual Testing Checklist
Before submitting a PR, please test:

**Basic Functionality:**
- [ ] File upload (drag & drop and click)
- [ ] Mod search and addition
- [ ] Platform/version selection
- [ ] Update button functionality
- [ ] Download generation (.mrpack and .zip)

**Error Handling:**
- [ ] Invalid file uploads
- [ ] Network connectivity issues
- [ ] API rate limit scenarios
- [ ] Large file processing

**Cross-Browser Testing:**
- [ ] Chrome (latest)
- [ ] Firefox (latest)
- [ ] Safari (if available)
- [ ] Edge (latest)

**Mobile Testing:**
- [ ] Responsive layout
- [ ] Touch interactions
- [ ] File upload on mobile
- [ ] Performance on slower devices

## 📋 Issue Guidelines

### Before Creating an Issue
1. **Search existing issues** to avoid duplicates
2. **Use the appropriate template** for your issue type
3. **Provide complete information** as requested in the template
4. **Use clear, descriptive titles**

### Issue Titles
**Good examples:**
- `Bug: ZIP download fails on large modpacks`
- `Feature: Add support for CurseForge mod imports`
- `Performance: Slow processing with 100+ mods`

**Avoid:**
- `It's broken`
- `Feature request`
- `Help me`

## 🔄 Pull Request Process

### PR Requirements
1. **Fill out the PR template** completely
2. **Reference related issues** using keywords:
   - `Fixes #123` (closes the issue)
   - `Addresses #123` (relates to the issue)
3. **Keep PRs focused** - one feature or bug fix per PR
4. **Update documentation** if needed
5. **Test your changes** thoroughly

### PR Review Process
1. **Automated checks** will run (if configured)
2. **Maintainer review** - we'll provide feedback
3. **Address feedback** promptly and professionally
4. **Final approval** and merge

### PR Title Format
- `feat: add bulk mod selection feature`
- `fix: resolve ZIP download timeout issue`
- `docs: update installation instructions`
- `perf: optimize large modpack processing`
- `style: improve mobile layout consistency`

## 💬 Community and Support

### Getting Help
- **GitHub Issues** - For bugs and feature requests
- **GitHub Discussions** - For general questions and community chat
- **Documentation** - Check the README first

### Stay Connected
- Watch the repository for updates
- Join discussions to help other users
- Share the project with the Minecraft community

### Recognition
Contributors will be:
- Listed in release notes for significant contributions
- Recognized in the README contributors section
- Thanked personally by the maintainers

## 📄 License

By contributing to MC Mod Updater, you agree that your contributions will be licensed under the [Mozilla Public License 2.0](LICENSE).

This means:
- Your contributions become part of the open-source project
- Others can use and modify your code
- Any changes to your code must remain open source
- Commercial use is allowed

---

## 🎉 Thank You!

Every contribution, no matter how small, helps make MC Mod Updater better for the entire Minecraft community. Whether you're fixing a typo, reporting a bug, or adding a major feature, your help is appreciated! 

**Happy coding!** 🚀

---

*Questions about contributing? Feel free to open an issue with the "question" label, and we'll help you get started!* 