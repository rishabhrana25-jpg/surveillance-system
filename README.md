# Smart Movable and Controlled Video-Based Surveillance Bot Management System

![Project Status](https://img.shields.io/badge/status-active-success.svg)
![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)

## 🎯 Project Overview

A comprehensive web-based management system for IoT surveillance bots with real-time sensor monitoring, user management, and security controls. Built as part of NIIT University B.Tech project.

## ✨ Features

### 🔐 User Authentication
- User registration with validation
- Secure login system
- Admin and User role separation
- Demo accounts for testing

### 📊 User Dashboard
- Real-time temperature & humidity monitoring
- Interactive Chart.js visualizations
- Auto-refresh sensor data (60s interval)
- Activity log tracking
- ThingSpeak API integration

### 👨‍💼 Admin Dashboard
- User management (Add, View, Delete users)
- Sensor configuration and management
- Analytics dashboard with charts
- Security controls (Alarm toggle, System lock)
- Activity logs with filtering
- CSV export for reports
- System summary generation

### 🛡️ Security Features
- Alarm system toggle
- System lock/unlock controls
- Security event logging
- Manual security checks
- Activity tracking

## 🚀 Installation & Setup

### Prerequisites
- Modern web browser (Chrome, Firefox, Edge, Safari)
- Text editor (VS Code recommended)
- Internet connection (for ThingSpeak API)

### Setup Steps

1. **Extract Files**
Extract all files to a folder with this structure:

project-folder/
├── index.html
├── user.html
├── admin.html
├── register.html
├── user-dashboard.html
├── admin-dashboard.html
├── style.css
├── README.md
└── assets/
├── niit-logo.png
├── robot.jpg
├── user.jpg
└── admin.jpg


2. **Open in Browser**
- Double-click `index.html` to launch
- Or use Live Server extension in VS Code

3. **ThingSpeak Configuration** (Optional)
- Open `user-dashboard.html`
- Find the configuration section:
  ```
  const CHANNEL_ID = 3118106;
  const READ_API_KEY = 'Z4MZRYY52ERGPPB5';
  ```
- Replace with your ThingSpeak credentials if needed

## 🔑 Login Credentials

### Admin Account
- **Username**: `admin`
- **Password**: `1234`

### Demo User Account
- **Email**: `demo@test.com`
- **Password**: `demo123`

### Create New User
- Click "Register" on the login page
- Fill in your details
- Login with your new account

## 📱 Usage Guide

### For Users
1. Login with user credentials
2. View real-time sensor data (temperature & humidity)
3. Monitor activity logs
4. Refresh data manually or wait for auto-update

### For Admins
1. Login with admin credentials
2. Navigate through 6 main sections:
- **User Management**: Add/remove users
- **Sensor Management**: Configure sensors
- **Analytics**: View data charts
- **Security**: Control alarms and locks
- **Reports**: Export data as CSV
- **Activity Logs**: Monitor system events

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Charts**: Chart.js
- **Storage**: LocalStorage API
- **IoT Integration**: ThingSpeak API
- **Icons**: Emoji-based (no external dependencies)

## 📂 File Structure

├── index.html # Landing page with role selection
├── user.html # User login page
├── admin.html # Admin login page
├── register.html # New user registration
├── user-dashboard.html # User dashboard with sensors
├── admin-dashboard.html # Complete admin panel
├── style.css # Global stylesheet
├── README.md # This file
└── assets/ # Images and resources


## 🎨 Features Breakdown

### User Dashboard
- 📊 Current temperature & humidity display
- 📈 Line charts for historical data
- 🔄 Auto-refresh every 60 seconds
- 📋 Activity log viewer
- 🗑️ Clear logs functionality

### Admin Dashboard
- 👥 **User Management**: CRUD operations
- 📡 **Sensor Management**: Add/remove sensors
- 📊 **Analytics**: Visual data representation
- 🔒 **Security Controls**: 
  - Toggle alarm (ON/OFF)
  - Lock/Unlock system
  - Manual security checks
- 📄 **Reports**: 
  - Export users to CSV
  - Export sensors to CSV
  - Generate system summary
- 📋 **Activity Logs**:
  - Filter by type (info, warning, error, success, sensor, security)
  - Export logs to CSV
  - Delete individual logs
  - Clear all logs

## 🔧 Customization

### Change ThingSpeak Channel
Edit `user-dashboard.html`:

const CHANNEL_ID = YOUR_CHANNEL_ID;
const READ_API_KEY = 'YOUR_API_KEY';


### Change Admin Credentials
Edit `admin.html`:

if (user === 'admin' && pass === '1234') {
// Change 'admin' and '1234' to your preferred credentials
}


### Adjust Auto-Refresh Interval
Edit `user-dashboard.html`:

const AUTO_REFRESH_SECONDS = 60; // Change to desired seconds


## 🐛 Troubleshooting

### Sensor Data Not Loading
- Check internet connection
- Verify ThingSpeak channel ID and API key
- Ensure channel is public or API key is correct
- Check browser console for errors (F12)

### Login Not Working
- Clear browser cache and localStorage
- Use correct credentials (see Login Credentials section)
- Try registering a new account

### Charts Not Displaying
- Ensure Chart.js CDN is accessible
- Check browser console for errors
- Verify sensor data is being received

## 📊 Browser Compatibility

✅ Chrome (Recommended)  
✅ Firefox  
✅ Edge  
✅ Safari  
⚠️ Internet Explorer (Not supported)

## 🎓 Academic Information

**Institution**: NIIT University  
**Course**: B.Tech (First Semester)  
**Project Type**: IoT Surveillance System  
**Technologies**: HTML, CSS, JavaScript, ThingSpeak  

## 📝 Notes

- Data stored in browser localStorage (persists locally)
- For production use, implement backend database
- Admin credentials should be changed for security
- Passwords are stored in plain text (demo purposes only)

## 🚀 Future Enhancements

- [ ] Backend integration with database
- [ ] User profile editing
- [ ] Password encryption
- [ ] Email notifications
- [ ] Mobile app version
- [ ] Live camera feed integration
- [ ] Bot movement controls
- [ ] Multi-language support

## 📧 Support

For issues or questions:
- Review this README thoroughly
- Check browser console (F12) for errors
- Verify all files are in correct locations
- Ensure internet connection for ThingSpeak

## 📜 License

This project is created for educational purposes as part of NIIT University coursework.

---

**Built with ❤️ for NIIT University**  
*Version 1.0.0 - October 2025*
