# Contributing to Contractor Time Tracker

First off, thank you for considering contributing to Contractor Time Tracker! 🎉

This project is developed and maintained by **Joseph Mark Orimoloye** at **Cybonix Solutions LLC**, and we welcome contributions from the community.

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Coding Standards](#coding-standards)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Features](#suggesting-features)

---

## 📜 Code of Conduct

### Our Pledge

We are committed to providing a welcoming and inclusive environment for everyone, regardless of:
- Age, body size, disability, ethnicity, gender identity and expression
- Level of experience, nationality, personal appearance, race, religion
- Sexual identity and orientation

### Our Standards

**Positive behavior includes:**
- Using welcoming and inclusive language
- Being respectful of differing viewpoints and experiences
- Gracefully accepting constructive criticism
- Focusing on what is best for the community
- Showing empathy towards other community members

**Unacceptable behavior includes:**
- Trolling, insulting/derogatory comments, and personal or political attacks
- Public or private harassment
- Publishing others' private information without explicit permission
- Other conduct which could reasonably be considered inappropriate

---

## 🤝 How Can I Contribute?

### Types of Contributions We Welcome

1. **🐛 Bug Reports**: Found a bug? Let us know!
2. **✨ Feature Requests**: Have an idea? Share it!
3. **📝 Documentation**: Improve or translate docs
4. **💻 Code Contributions**: Fix bugs or add features
5. **🎨 Design Improvements**: UI/UX enhancements
6. **🧪 Testing**: Help test new features
7. **🌍 Translations**: Make the app accessible in other languages

---

## 💻 Development Setup

### Prerequisites

Since this is a single-file HTML application, setup is minimal:

1. **Text Editor**: VS Code, Sublime, Atom, or any code editor
2. **Web Browser**: Chrome, Firefox, Edge, or Safari
3. **Git**: For version control

### Getting Started

```bash
# Fork the repository on GitHub

# Clone your fork
git clone https://github.com/Cybonix-Solutions/Contractor-Time-Tracker.git

# Navigate to the directory
cd Contractor-Time-Tracker

# Create a new branch for your feature
git checkout -b feature/your-feature-name

# Open time-tracker.html in your editor and browser
# Make your changes and test in the browser

# Test thoroughly
# - Try all features
# - Test on different screen sizes
# - Check browser console for errors
# - Test data persistence (refresh page)
```

### Testing Your Changes

1. Open `time-tracker.html` in your browser
2. Test all affected features thoroughly
3. Try different themes
4. Test on mobile/tablet (responsive design)
5. Check browser console for errors
6. Verify localStorage persistence (refresh page)
7. Test backup/restore functionality
8. Generate invoices and verify formatting

---

## 📐 Coding Standards

### JavaScript/React
- Use functional components with hooks
- Use `memo` for components that shouldn't re-render unnecessarily
- Keep functions focused and single-purpose
- Add comments for complex logic
- Use meaningful variable names

### CSS
- Use CSS variables for theme colors
- Follow existing naming conventions
- Ensure responsive design (mobile-first approach)
- Test on different screen sizes
- Maintain accessibility (WCAG guidelines)

### Code Style
```javascript
// ✅ Good
const calculateHours = (session) => {
    if (!session.startTime || !session.endTime) return 0;
    // ... calculation logic
};

// ❌ Avoid
function calc(s){return s.e-s.s}
```

### Comments
```javascript
// ✅ Good - Explain WHY, not WHAT
// Prevent save operations during initial data load from localStorage
if (!isInitialLoad) {
    localStorage.setItem('workSessions', JSON.stringify(workSessions));
}

// ❌ Avoid - States the obvious
// Set work sessions in local storage
localStorage.setItem('workSessions', JSON.stringify(workSessions));
```

---

## 📝 Commit Guidelines

### Commit Message Format

Use clear, descriptive commit messages:

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

### Examples

```bash
feat(themes): add sunset theme with orange gradient

Added new "Sunset Blaze" theme with orange to pink gradient.
Updated theme selector to include the new option.

Closes #42

---

fix(invoice): correct currency formatting in Excel export

Fixed issue where amounts over $1,000 weren't displaying
with comma separators. Updated XLSX number format.

Fixes #38

---

docs(readme): add troubleshooting section

Added common issues and solutions to README.
Includes localStorage quota errors and import failures.
```

---

## 🔄 Pull Request Process

### Before Submitting

1. ✅ Test your changes thoroughly
2. ✅ Update documentation if needed
3. ✅ Add your changes to CHANGELOG.md
4. ✅ Ensure no console errors
5. ✅ Test on multiple browsers
6. ✅ Verify responsive design

### Submitting a Pull Request

1. **Push your branch** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create Pull Request** on GitHub:
   - Use a clear title
   - Reference any related issues
   - Describe what changed and why
   - Include screenshots for UI changes
   - List any breaking changes

3. **Pull Request Template**:
   ```markdown
   ## Description
   Brief description of changes
   
   ## Type of Change
   - [ ] Bug fix
   - [ ] New feature
   - [ ] Documentation update
   - [ ] Code refactoring
   
   ## Testing
   - [ ] Tested in Chrome
   - [ ] Tested in Firefox
   - [ ] Tested on mobile
   - [ ] Tested data persistence
   
   ## Screenshots (if applicable)
   
   ## Related Issues
   Fixes #(issue number)
   
   ## Checklist
   - [ ] My code follows the style guidelines
   - [ ] I have commented complex code
   - [ ] I have updated documentation
   - [ ] I have added to CHANGELOG.md
   - [ ] My changes generate no console errors
   ```

### Review Process

1. Maintainer will review your PR
2. Feedback may be provided
3. Make requested changes if needed
4. Once approved, PR will be merged
5. Your contribution will be credited!

---

## 🐛 Reporting Bugs

### Before Submitting a Bug Report

1. Check existing issues
2. Test in latest browser version
3. Clear localStorage and test again
4. Try in incognito/private mode

### Bug Report Template

```markdown
**Bug Description**
A clear description of the bug

**Steps to Reproduce**
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected Behavior**
What should happen

**Actual Behavior**
What actually happened

**Screenshots**
If applicable

**Environment**
- Browser: [e.g., Chrome 120]
- OS: [e.g., Windows 11, macOS 14]
- App Version: [e.g., 1.0.0]

**Additional Context**
Any other relevant information
```

---

## ✨ Suggesting Features

### Before Suggesting

1. Check if feature already exists
2. Search existing feature requests
3. Consider if it fits project scope

### Feature Request Template

```markdown
**Feature Description**
Clear description of the proposed feature

**Problem It Solves**
What problem does this feature address?

**Proposed Solution**
How would you implement this?

**Alternatives Considered**
What other solutions did you consider?

**Additional Context**
Mockups, examples, etc.

**Priority**
Low / Medium / High

**Willing to Contribute**
Yes / No / Need guidance
```

---

## 🎯 Priority Areas

We especially welcome contributions in these areas:

### High Priority
- 🐛 Bug fixes
- 📱 Mobile experience improvements
- ♿ Accessibility enhancements
- 🌍 Internationalization (i18n)

### Medium Priority
- ✨ New themes
- 📊 Additional export formats
- 📈 Data visualization
- ⌨️ Keyboard shortcuts

### Low Priority
- 🎨 UI polish
- 📝 Documentation improvements
- 🧪 Testing utilities

---

## 📞 Getting Help

Need help contributing? Reach out:

- 💬 Open a [GitHub Discussion](https://github.com/Cybonix-Solutions/Contractor-Time-Tracker/discussions)
- 🐛 Check [existing issues](https://github.com/Cybonix-Solutions/Contractor-Time-Tracker/issues)
- 📧 Contact: [Create an issue](https://github.com/Cybonix-Solutions/Contractor-Time-Tracker/issues/new)

---

## 🏆 Recognition

Contributors will be:
- Listed in README.md
- Credited in release notes
- Mentioned in CHANGELOG.md
- Given a shout-out on social media (if desired)

---

## 📜 License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

## 🙏 Thank You!

Every contribution, no matter how small, is valuable and appreciated. Thank you for helping make Contractor Time Tracker better for everyone!

---

**Maintained by Joseph Mark Orimoloye**  
**© 2025 Cybonix Solutions LLC**

---

*This document is inspired by open-source contribution guidelines from various successful projects.*
