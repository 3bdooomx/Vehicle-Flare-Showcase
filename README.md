# 🚗 FareFlow - Vehicle Fare Management App

A modern, highly responsive Flutter application designed for calculating, managing, and visualizing vehicle fare structures, interactive seating layouts, and custom rate configurations.

---

## 🏗️ Architecture & State Management

This project follows a **Layered Architecture (Separation of Concerns)** to ensure scalability, maintainability, and clean code principles.

* **Architecture Pattern**: Layered Architecture separating models, providers, screens, widgets, and utilities.
* **State Management**: **Provider Pattern (`ChangeNotifier` + `provider`)** delivering reactive UI updates and efficient state propagation across screens.
* **Local Persistence**: Integrated `SharedPreferences` for persisting user preferences and application configuration.
* **Localization & Theming**: Dedicated design system and multi-language translation management.

---

## 📂 Directory Structure

```text
fare_flow/
├── assets/                       # Static assets and icons
│   └── icons/                    # App iconography
├── lib/                          # Main application source code
│   ├── models/                   # Domain models and data entities
│   │   ├── seat.dart             # Model defining seat attributes and states
│   │   └── vehicle.dart          # Model representing vehicle configurations and rates
│   ├── providers/                # State management and core business logic
│   │   └── app_provider.dart     # App state manager and data persistence driver
│   ├── screens/                  # Presentation layer and application screens
│   │   ├── splash_screen.dart             # App launch and initialization screen
│   │   ├── vehicle_selection_screen.dart # Vehicle selection interface
│   │   ├── seat_layout_screen.dart        # Interactive seating arrangement layout view
│   │   ├── fare_input_screen.dart         # Fare calculation and rate configuration view
│   │   ├── summary_screen.dart            # Trip and fare calculation summary view
│   │   └── settings_screen.dart           # Preferences and settings view
│   ├── utils/                    # Shared utilities, app themes, and localization
│   │   ├── theme.dart            # Color palettes, typography, and visual design rules
│   │   └── translations.dart     # Multi-language string dictionaries
│   ├── widgets/                  # Modular, reusable custom UI components
│   │   ├── animated_number.dart  # Custom animated counter widget
│   │   └── app_background.dart   # Reusable styled visual background container
│   └── main.dart                 # Application entry point and provider setup
├── analysis_options.yaml         # Linting and static analysis configuration
└── pubspec.yaml                  # Dependencies, assets, and project metadata
```

---

## 🛠️ Tech Stack & Key Packages

* **Framework**: [Flutter](https://flutter.dev/) (Dart SDK >=3.0.0 <4.0.0)
* **State Management**: [`provider`](https://pub.dev/packages/provider) (^6.1.1)
* **Local Storage**: [`shared_preferences`](https://pub.dev/packages/shared_preferences) (^2.2.2)
* **Animations**: [`flutter_animate`](https://pub.dev/packages/flutter_animate) (^4.3.0)
* **Iconography**: [`font_awesome_flutter`](https://pub.dev/packages/font_awesome_flutter) & `cupertino_icons`
* **Localization**: `flutter_localizations`

---


