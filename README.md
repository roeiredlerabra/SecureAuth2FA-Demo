# SecureAuth2FA-Demo 🔐

A clean, user-friendly demonstration of Two-Factor Authentication (2FA) implementation using Google Authenticator. Built with pure HTML, JavaScript, and Bootstrap, this demo showcases a complete 2FA workflow without server dependencies.

![2FA Demo Screenshot](screenshots/demo.png) <!-- You can add screenshots later -->

## 🌟 Features

- **Complete 2FA Workflow**: Registration, Login, and Verification
- **Google Authenticator Integration**: Compatible with Google Authenticator and similar TOTP apps
- **Clean Bootstrap UI**: Step-by-step interface with visual guidance
- **Client-Side Implementation**: No server required, perfect for learning and demonstration
- **QR Code Generation**: Easy setup with Google Authenticator
- **Backup Code Support**: Manual entry option available
- **Responsive Design**: Works on both desktop and mobile devices

## 🚀 Quick Start

1. Clone the repository:
```bash
git clone https://github.com/yourusername/SecureAuth2FA-Demo.git
```

2. Open `index.html` in your web browser

No additional setup or installation required!

## 📱 Prerequisites

To test the 2FA functionality, you'll need:
- Google Authenticator app ([Android](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2) | [iOS](https://apps.apple.com/us/app/google-authenticator/id388497605))
- Or any TOTP-compatible authenticator app

## 🔍 How It Works

1. **Registration**
   - User creates an account
   - System generates a unique secret key
   - QR code is displayed for Google Authenticator setup

2. **Login**
   - User enters credentials
   - First-factor authentication completed

3. **2FA Verification**
   - User enters 6-digit code from Google Authenticator
   - Time-based One-Time Password (TOTP) verification
   - Access granted upon successful verification

## 💻 Technical Implementation

- **TOTP Implementation**: Uses HMAC-SHA1 for token generation
- **Storage**: Utilizes localStorage for demo purposes (not for production use)
- **Libraries Used**:
  - Bootstrap 5.3.0
  - CryptoJS 4.1.1
  - QRCode.js 1.0.0

## ⚠️ Important Notes

This is a demonstration project and shouldn't be used in production as-is because:
- Passwords are stored in plain text
- Uses localStorage instead of secure server storage
- No session management
- No rate limiting
- No password hashing

For production use, implement proper security measures including:
- Secure server-side storage
- Password hashing
- Rate limiting
- Session management
- HTTPS
- Proper error handling

## 🔧 Development

Want to contribute? Great! Here are some areas for improvement:
- Add server-side implementation
- Implement password hashing
- Add rate limiting
- Add backup codes functionality
- Add session management
- Add tests

## 📄 License

MIT License - feel free to use this demo for learning purposes!

## 👏 Credits

Created by [Your Name]

## 📧 Contact

- GitHub: [@yourusername](https://github.com/yourusername)
- Email: your.email@example.com

---

Made with ❤️ for the developer community
