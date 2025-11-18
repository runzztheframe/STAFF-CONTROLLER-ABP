🏢 Staff Management System - ប្រព័ន្ធគ្រប់គ្រងបុគ្គលិក

A modern, professional staff management system built with Python and Tkinter, featuring a beautiful Khmer language interface and comprehensive employee management capabilities.

✨ Features

👥 Core Staff Management
- Complete Employee Profiles - Store name, position, department, salary, contact info
- Photo Management - Upload and preview staff photos with automatic optimization
- Document Storage - Attach PDFs, DOCX files to employee records
- Birthday Tracking - Automatic birthday reminders and age calculation
- Department Organization - Filter and organize staff by departments

🎨 Modern User Interface
- Dark/Light Themes - Professional color schemes with instant switching
- Khmer Language Support - Full localization with Khmer interface
- Real-time Clock - Live time and date display
- Interactive Calendar - Monthly view with staff birthday highlights
- Responsive Design - Adapts to different screen sizes

📊 Advanced Features
- Smart Search & Filter - Quick search by name, position, or department
- Excel Export - Professional reports with formatting and auto-adjust columns
- Data Backup - Automatic backup system with configurable retention
- Statistics Dashboard - Real-time staff and department counts

⚙️ Professional Settings
- Comprehensive Configuration - 7 categories of settings
- Theme Customization - Dark/light mode with live preview
- Security Settings - Multiple security levels and session timeouts
- Export Options - Excel, PDF, CSV format support
- Company Branding - Custom company name and defaults

🚀 Installation

Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

Required Packages
pip install pillow pandas openpyxl matplotlib seaborn python-dateutil

Quick Start
1. Clone or download the project files
2. Run the application:
python staff_management.py

3. First-time Setup:
   - The system will prompt for a data folder location
   - Choose any folder to store your staff data
   - Use any username/password to login (demo mode)

📖 User Guide

Adding Staff Members
1. Click the "📋 បញ្ជីបុគ្គលិក" (Staff List) tab
2. Fill in the form on the left side:
   - Required: Full Name
   - Optional: Birthdate, Position, Salary, etc.
3. Click "➕ បន្ថែម" (Add) to save

Managing Photos & Documents
- Photos: Click "📁 ជ្រើសរូប" to select staff photos
- Preview: Click "👀 មើល" to view current photo
- Documents: Use document browser to attach files

Searching & Filtering
- Quick Search: Type in search box to filter by name/position
- Department Filter: Use dropdown to view specific departments
- Double-click any staff member to load their details

Calendar & Birthdays
1. Go to "📅 ប្រតិទិន" (Calendar) tab
2. Navigate months with arrow buttons
3. Click any date to see staff birthdays
4. View monthly birthdays in the bottom section

Exporting Data
1. Click "📊 Excel" button in staff list
2. Choose save location and filename
3. System generates formatted Excel report
4. Open automatically or save for later

Customizing Settings
1. Click "⚙️ ការកំណត់" (Settings) tab
2. Explore different categories:
   - ទូទៅ (General): Language, date format, currency
   - រូបរាង (Appearance): Themes, colors
   - ទិន្នន័យ (Data): Backup settings, storage location
   - នាំចេញ (Export): File formats, templates
   - សុវត្ថិភាព (Security): Access controls, timeouts
   - ក្រុមហ៊ុន (Company): Branding, defaults

🗂️ Database Structure

The system uses SQLite with the following main table:

staff(
  id INTEGER PRIMARY KEY,
  name TEXT NOT NULL,
  birthdate TEXT,
  marital_status TEXT,
  location TEXT,
  position TEXT,
  salary REAL,
  hire_date TEXT,
  phone TEXT,
  email TEXT,
  department TEXT,
  photo_path TEXT,
  document_path TEXT,
  created_date TEXT,
  last_updated TEXT
)

🎯 Keyboard Shortcuts

- Double-click staff in list - Edit staff details
- Enter in search box - Quick search
- Ctrl+S - Quick save current form
- Esc - Close dialogs and popups

🔧 Technical Details

File Structure
staff_management.py      # Main application
config.json             # User settings and preferences
/data_folder/           # Your chosen data location
  ├── staff_data.db     # SQLite database
  ├── Photos/           # Staff photos
  ├── Documents/        # Attached documents
  └── Backups/          # Automatic backups

Supported Image Formats
- JPEG (.jpg, .jpeg)
- PNG (.png)
- BMP (.bmp)
- GIF (.gif)

Supported Document Formats
- PDF (.pdf)
- Word Documents (.docx)
- All files (.*)

🛠️ Customization

Adding New Departments
Edit the department list in the form creation section:

values = ["IT", "លក់", "ទីផ្សារ", "HR", "ហិរញ្ញវត្ថុ", "ផ្សេងៗ"]

Modifying Themes
Edit color schemes in the COLORS dictionary:

COLORS = {
    "primary": "#6366f1",
    "background": "#0f172a",
    # ... more colors
}

📞 Support

Common Issues
1. "Database Error" - Ensure write permissions in data folder
2. "Photo not loading" - Check image format and file permissions
3. "Export failed" - Close Excel file if open, check disk space

Troubleshooting
- Reset Settings: Use "🔄 កំណត់ឡើងវិញ" in settings
- Change Data Folder: Use settings to relocate data
- Manual Backup: Copy the entire data folder

📄 License

This project is licensed under the MIT License.

🔄 Version History

- v2.0 (Current) - Professional settings, calendar, real-time clock
- v1.0 - Basic staff management with Khmer interface

👥 Contributing

We welcome contributions! Please feel free to submit pull requests or open issues for:
- Bug fixes
- New features
- Translation improvements
- Documentation updates

🏢 About

This staff management system is designed for Cambodian businesses and organizations needing a simple, effective way to manage employee information with full Khmer language support.

---

Note: This is a demo system. For production use, consider adding user authentication and database encryption based on your security requirements.

Happy Staff Managing! 🎉

📸 Screenshots

(Add your screenshots here when you upload them to GitHub)

- Login Screen with Khmer interface
- Main Staff Management Dashboard
- Calendar View with Birthday Highlights
- Professional Settings Panel
- Excel Export Example

---

Made with ❤️ for Cambodian Businesses

If you find this project helpful, please give it a ⭐!
