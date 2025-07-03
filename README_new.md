# 💰 Smart Wallet & Expense Tracker

[![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev/)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Wear OS](https://img.shields.io/badge/Wear%20OS-4285F4?style=for-the-badge&logo=wear-os&logoColor=white)](https://wearos.google.com/)

A comprehensive cross-platform personal finance application designed to help users track expenses, set budgets, and monitor financial health in real-time across Wear OS smartwatch, Android smartphone, and Windows laptop.

## 🎯 Project Overview

The Smart Wallet & Expense Tracker is a unified financial tracking system that provides seamless synchronization across multiple devices. Users can quickly add expenses on their smartwatch, view detailed analytics on their phone, and perform advanced planning on their desktop.

### 🚀 Key Features

- **Real-time Cross-Platform Sync** - Instant data synchronization across all devices
- **Quick Expense Entry** - Voice input and predefined categories on smartwatch
- **Advanced Analytics** - Comprehensive reports and visualizations
- **Offline Support** - Local storage with background sync
- **Smart Insights** - AI-powered spending pattern analysis
- **Secure Authentication** - Firebase Auth with biometric support

## 🏗️ Tech Stack

- **Frontend**: Flutter (Mobile, Desktop, Wear OS)
- **Backend**: Firebase (Firestore, Authentication)
- **Local Storage**: SQLite
- **Authentication**: Firebase Auth, Google OAuth 2.0
- **Analytics**: Charts and data visualization libraries

## 📱 Platform Support

### 🕶️ Wear OS Watch
- Quick expense addition via voice input
- Predefined spending categories
- Daily spending overview
- Haptic feedback for budget alerts
- Weekly budget limit notifications

### 📱 Android Phone
- Complete user authentication system
- Full expense management (add, edit, delete)
- Receipt capture with OCR integration
- Recurring bills setup
- Visual reports (pie charts, bar graphs)
- Budget planning and tracking
- Offline mode with automatic sync

### 💻 Windows Desktop
- Comprehensive financial dashboard
- Advanced reporting and analytics
- Multi-month budget planning
- Export functionality (PDF, Excel)
- Goal tracking and planning
- Family/team wallet sharing

## 🔐 Security & Authentication

- **Firebase Authentication** with multiple sign-in options:
  - Google Sign-in (OAuth 2.0)
  - Email/Password
  - OTP verification
- **Biometric Authentication** (fingerprint, face unlock)
- **Secure Firestore Rules** for user data protection
- **End-to-end encryption** for sensitive financial data

## 📊 Expense Categories

| Category | Description |
|----------|-------------|
| 🍕 Food & Drinks | Restaurants, groceries, beverages |
| 🚗 Transportation | Gas, public transport, ride-sharing |
| 🛍️ Shopping | Clothing, electronics, general purchases |
| 🎬 Entertainment | Movies, games, subscriptions |
| 💡 Utilities & Bills | Electricity, water, internet, phone |
| 🏥 Health & Fitness | Medical, gym, wellness |
| 📂 Others | Miscellaneous expenses |

*Categories are fully customizable by users*

## 🔄 Data Synchronization

### Cloud Storage
- **Primary**: Firebase Firestore for real-time sync
- **Backup**: Automatic cloud backups with version control

### Offline Support
- **Local Database**: SQLite for offline functionality
- **Sync Engine**: Intelligent conflict resolution
- **Background Sync**: Automatic synchronization when online
- **Manual Refresh**: User-triggered sync option

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (3.0 or higher)
- Android Studio / VS Code
- Firebase project setup
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/smartwallet.git
   cd smartwallet
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Firebase Setup**
   - Create a new Firebase project
   - Add Android and Web apps to your project
   - Download and place configuration files:
     - `android/app/google-services.json`
     - `web/firebase-config.js`

4. **Run the application**
   ```bash
   # For Android
   flutter run

   # For Windows Desktop
   flutter run -d windows

   # For Wear OS (requires paired device)
   flutter run -d wear
   ```

## 📁 Project Structure

```
smartwallet/
├── lib/
│   ├── common/           # Shared models, utilities, constants
│   │   ├── models/       # Data models (Expense, User, Budget)
│   │   ├── services/     # Business logic services
│   │   └── utils/        # Helper functions and utilities
│   ├── mobile/           # Android-specific UI and features
│   │   ├── screens/      # Mobile app screens
│   │   ├── widgets/      # Reusable mobile widgets
│   │   └── controllers/  # Mobile-specific controllers
│   ├── desktop/          # Windows desktop UI and features
│   │   ├── screens/      # Desktop app screens
│   │   ├── widgets/      # Desktop-specific widgets
│   │   └── controllers/  # Desktop controllers
│   ├── watch/            # Wear OS interface
│   │   ├── screens/      # Watch app screens
│   │   └── widgets/      # Watch-specific widgets
│   ├── services/         # Core services
│   │   ├── auth_service.dart
│   │   ├── database_service.dart
│   │   ├── sync_service.dart
│   │   └── notification_service.dart
│   └── main.dart         # Application entry point
├── assets/               # Images, icons, fonts
├── test/                 # Unit and widget tests
├── integration_test/     # Integration tests
├── android/              # Android-specific configuration
├── windows/              # Windows-specific configuration
├── wear/                 # Wear OS configuration
├── web/                  # Web platform files
├── pubspec.yaml          # Dependencies and project configuration
└── README.md             # This file
```

## 🧪 Testing

Run tests using the following commands:

```bash
# Unit tests
flutter test

# Integration tests
flutter test integration_test/

# Test coverage
flutter test --coverage
```

## 📦 Building for Production

### Android APK
```bash
flutter build apk --release
```

### Windows Desktop
```bash
flutter build windows --release
```

### Wear OS
```bash
flutter build apk --target-platform android-arm64 --release
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📋 Development Roadmap

- [x] Project setup and structure
- [ ] Firebase authentication integration
- [ ] Core expense tracking functionality
- [ ] Android mobile app development
- [ ] Windows desktop application
- [ ] Wear OS interface
- [ ] Cross-platform synchronization
- [ ] Advanced analytics and reporting
- [ ] AI-powered insights
- [ ] Export functionality
- [ ] Multi-user support

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For support, email support@smartwallet.com or join our Slack channel.

## 🙏 Acknowledgments

- Flutter team for the amazing framework
- Firebase for backend services
- Contributors and beta testers
- Open source community

---

**Made with ❤️ using Flutter**
