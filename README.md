# ⏱️ Contractor Time Tracker

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

A professional, feature-rich time tracking and invoicing application for contractors and freelancers. Built with React and designed for simplicity and privacy - all data stays local on your device.

**Developed by [Joseph Mark Orimoloye](https://github.com/Cybonix)**  
**© 2025 Cybonix Solutions LLC**

---

## 🌟 Features

### Time Tracking
- ⏰ **Real-time clock** with live session tracking
- 🟢 **Start/Stop work sessions** with automatic time calculation
- ☕ **Break management** with optional reasons and duration tracking
- 📝 **Session notes** for detailed work documentation
- 🔄 **Manual entry** for adding historical work sessions

### Session Management
- ✏️ **Edit entries** - Modify any session within 14 days
- 📅 **Date/time editing** with full validation
- 🛑 **Break editing** - Add, remove, or modify breaks
- 🔒 **14-day lock** prevents editing of older sessions for data integrity

### Professional Invoicing
- 📊 **Excel invoices** with professional formatting and conditional styling
- 📈 **CSV exports** for easy importing into accounting software
- 💼 **Customizable billing information** (contractor and client details)
- 💰 **Configurable hourly rates**
- 📋 **Comprehensive reports** (daily, weekly, bi-weekly, custom ranges)

### User Experience
- 🎨 **7 beautiful themes** with smooth color transitions
- 📱 **Fully responsive** - works on desktop, tablet, and mobile
- 💾 **Local data storage** - complete privacy, no cloud required
- 📤 **Backup/restore** functionality (JSON export/import)
- 🔄 **Backward compatible** with older backup formats

---

## 🚀 Quick Start

### Installation

1. **Download the HTML file**
   ```bash
   git clone https://github.com/Cybonix-Solutions/Contractor-Time-Tracker.git
   cd contractor-time-tracker
   ```

2. **Open in your browser**
   - Simply double-click `time-tracker.html`
   - Or drag and drop the file into your browser
   - No installation, no setup required!

### First-Time Setup

1. **Set up billing information**
   - Click on the **Settings** tab
   - Enter your contractor information (name, address, contact details)
   - Enter your client information
   - Set your hourly rate
   - Click **Save**

2. **Choose your theme** (optional)
   - Click one of the 7 color circles in the top-right corner
   - Your theme choice will be saved automatically

3. **Start tracking time!**
   - Go to the **Time Tracker** tab
   - Click **Start Work Day**
   - Use **Start Break** and **Return from Break** as needed
   - Click **End Work Day** when finished

---

## 📖 User Guide

### Time Tracker Tab
Track your work in real-time with intuitive controls:
- **Start Work Day**: Begin a new work session
- **Start Break**: Log unpaid breaks (lunch, personal time, etc.)
- **Return from Break**: Resume working
- **End Work Day**: Complete the session and save

### Manual Entry Tab
Add historical work sessions:
- Select the date and times
- Add breaks with durations and reasons
- Include optional notes
- See real-time hour calculations

### Work History Tab
Review all your tracked sessions:
- View sessions sorted by date (newest first)
- See detailed breakdown of hours, breaks, and notes
- **Edit** recent sessions (within 14 days)
- Sessions older than 14 days are locked for data integrity

### Reports & Invoices Tab
Generate professional billing documents:
- Choose report period (today, last 7 days, last 14 days, or custom)
- View summary statistics (sessions, hours, amount)
- Generate **Excel invoices** with professional formatting
- Export **CSV reports** for accounting software

### Settings Tab
Manage your app and data:
- **Edit billing information** (contractor, client, hourly rate)
- **Export backup** (save your data as JSON)
- **Import backup** (restore from previous backup)
- **Clear all data** (reset to defaults)

---

## 🎨 Themes

Choose from 7 beautiful gradient themes:
1. **Purple Majesty** - Classic purple/violet (default)
2. **Ocean Breeze** - Calming blue gradients
3. **Sunset Blaze** - Warm red to pink
4. **Forest Green** - Natural teal to green
5. **Royal Gold** - Elegant navy to gold
6. **Berry Blast** - Vibrant purple/violet
7. **Rose Garden** - Deep red to magenta

All themes feature smooth 0.3-0.5 second transitions and affect headers, buttons, and accent colors throughout the app.

---

## 📊 Invoice & Export Features

### Excel Invoice
Professional invoices include:
- Complete contractor and client information
- Detailed session breakdown with dates and times
- Break information with durations and reasons
- Session notes
- Professional formatting with:
  - Color-coded headers (purple background, white text)
  - Alternating row colors for readability
  - Highlighted break information (yellow background)
  - Bold totals with professional borders
  - Text wrapping for notes and break details
  - Currency formatting

### CSV Export
Flat-structure exports perfect for importing:
- Columns: Date, Day, Start Time, End Time, Break Count, Total Break Minutes, Break Details, Hours, Rate, Amount, Notes
- Properly escaped for compatibility
- Summary row with totals
- Easy to import into Excel, Google Sheets, QuickBooks, etc.

---

## 💾 Data Storage & Privacy

### Local Storage
- All data is stored in your browser's **localStorage**
- **No cloud services** - complete privacy
- **No tracking** - no analytics or data collection
- **No account required** - just download and use

### Data Safety
⚠️ **Important**: Browser data can be cleared or lost. We strongly recommend:
- Regular backups using the **Export Backup** feature
- Storing backup files in a safe location
- Exporting invoices promptly after each billing period

### Backup & Restore
- **Export**: JSON file with all sessions and settings
- **Import**: Restore from any backup file
- **Backward compatible**: Automatically converts older backup formats

---

## 🔧 Technical Details

### Technology Stack
- **Frontend**: React 18 (via CDN)
- **Styling**: Pure CSS with CSS Variables for theming
- **Excel Generation**: SheetJS (XLSX library)
- **Storage**: Browser localStorage API
- **No Backend**: Completely client-side application

### Browser Compatibility
Works on all modern browsers:
- ✅ Chrome/Edge (Recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Opera

### File Structure
```
contractor-time-tracker/
├── time-tracker.html       # Main application (single file)
├── README.md              # This file
├── LICENSE                # MIT License
├── CHANGELOG.md           # Version history
├── CONTRIBUTING.md        # Contribution guidelines
└── .gitignore            # Git ignore rules
```

---

## 🤝 Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

Areas where you can help:
- 🐛 Bug fixes
- ✨ New features
- 📝 Documentation improvements
- 🌍 Translations
- 🎨 UI/UX enhancements

---

## 📝 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```
Copyright © 2025 Joseph Mark Orimoloye | Cybonix Solutions LLC

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## ⚠️ Disclaimer

This software is provided "as-is" without warranty of any kind. Users are responsible for:
- Verifying the accuracy of all time tracking and billing information
- Maintaining regular backups of their data
- Ensuring compliance with their local tax and labor laws
- Keeping their browser and system updated for optimal security

**Cybonix Solutions LLC** and **Joseph Mark Orimoloye** are not liable for any data loss, billing errors, or other issues arising from the use of this software.

---

## 📞 Support & Contact

**Developer**: Joseph Mark Orimoloye  
**Company**: Cybonix Solutions LLC  
**GitHub**: [@Cybonix](https://github.com/Cybonix)  
**Issues**: [Email: Cybonix Solutions](mailto:jorimoloye@cybonixsolutions.com)

For bug reports, feature requests, or questions, please open an issue on GitHub.

---

## 🙏 Acknowledgments

- React team for the excellent UI library
- SheetJS for Excel file generation
- The open-source community for inspiration and support

---

## 📈 Version History

See [CHANGELOG.md](CHANGELOG.md) for detailed version history.

**Current Version**: 1.0.0 (November 2025)

---

<div align="center">

**Built with ❤️ by Joseph Mark Orimoloye**

**© 2025 Cybonix Solutions LLC. All rights reserved.**

⭐ If you find this useful, please star the repository!

</div>
