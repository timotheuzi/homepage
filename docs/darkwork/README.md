# Dark Work Labs

**Package Name:** `com.darkwork.labs`  
**Version:** 1.0.0+1  
**Platform:** Android & Linux  
**Framework:** Flutter (Dart ≥ 3.0)

A comprehensive security monitoring application built with Flutter, designed for Android and Linux. Dark Work Labs acts as a digital sentinel, providing real-time oversight of your digital and physical environment.

**All data processing and storage occurs exclusively on your device; no data is ever transmitted or saved outside of your phone.**

## 🚀 Overview

Dark Work Labs provides real-time oversight of your digital and physical environment. Under the watchful eye of the **Great Defender** — a custom-painted Sentinel Shield icon featuring a deep obsidian shield, premium gold frame, and amethyst iris — it monitors network traffic, Bluetooth signals, and hardware sensor data.

## ✨ Features

### 🔍 Network & WiFi Sentinel
- **Automated Reconnaissance**: Scans local networks for nodes and open ports.
- **WiFi Security**: Detects Rogue Access Points, Evil Twin attacks, and unencrypted networks.

### 📡 Bluetooth & RF Surveillance
- **AirTag Identification**: Monitors BLE for Apple AirTags and Find My network-enabled trackers.
- **RF Spectrum Monitor**: Integration with external SDR hardware (RTL-SDR) to detect Sub-GHz surveillance signals.

### 📊 Hardware Telemetry
- **Real-time Streams**: Live monitoring of Accelerometer, Gyroscope, Magnetometer, and Ambient Light.
- **System Vitals**: Detailed tracking of CPU, memory, battery health, and active network sockets.

### 📁 File Integrity Scanner
- **Deep Analysis**: Scans local file systems for suspicious patterns, dangerous extensions, and risk indicators.
- **Risk Classification**: Categorises findings as Low, Medium, or High risk with detailed metadata.

### 📝 Logging & Intelligence
- **System Event Logs**: Real-time and historical log entries with date filtering and level-based colour coding.

## 🎨 The Great Defender UI
- **Unified Dashboard**: Real-time security status provided by the Sentinel Shield with gradient status header.
- **Premium Design Language**: Consistent, refined visual identity across all security modules with a centralised colour palette (`AppColors`).
- **Dark & Light Themes**: Beautifully crafted Material 3 themes with amethyst/cyan accent colours and gold shield framing.
- **Responsive Layouts**: Adaptive screens with scrollable empty states and loading indicators.

## 🏗️ Architecture

### State Management
- **Provider** (`package:provider`) — `ChangeNotifier` + `MultiProvider` pattern.
- All services extend `ChangeNotifier` and are registered in `main.dart`.

### Services (`lib/services/`)
| Service | Responsibility |
|---------|---------------|
| `SecurityService` | Core security monitoring, device discovery |
| `NetworkSecurityService` | Network scanning, port discovery |
| `SensorService` | Hardware sensor data collection (accelerometer, gyroscope, etc.) |
| `SystemMonitorService` | System vitals: CPU, memory, battery, network connections |
| `RadioFrequencyService` | SDR hardware detection and RF spectrum monitoring |
| `FilesystemScannerService` | File system integrity scanning and risk analysis |
| `LoggingService` | Centralised event logging with historical retrieval |
| `DatabaseService` | Local SQLite database for persistent storage |
| `ThemeService` | Centralised theming with `AppColors` palette |

### Models (`lib/models/`)
| Model | Description |
|-------|-------------|
| `Device` | Network, Bluetooth, WiFi, and AirTag device data |

### Screens (`lib/screens/`)
| Screen | Purpose |
|--------|---------|
| `DashboardScreen` | Main command center with status header, quick stats |
| `DeviceListScreen` | Discovered device management with filtering |
| `NetworkSecurityScreen` | Network scanner, security report, and logs (tabbed) |
| `SensorMonitorScreen` | Real-time hardware sensor telemetry |
| `SystemMonitorScreen` | System vitals, network identity, and active sockets |
| `RadioMonitorScreen` | RF spectrum monitoring and SDR device detection |
| `FilesystemScannerScreen` | File integrity scanning with risk classification |
| `LoggingScreen` | System event logs with date filtering and level colours |
| `SettingsScreen` | System settings and appearance configuration |

### Widgets (`lib/widgets/`)
| Widget | Description |
|--------|-------------|
| `AncientShieldIcon` | Custom-painted Sentinel Shield with gold frame and amethyst iris |

## 🔧 Build & Development

### Prerequisites
- Flutter SDK ≥ 3.0
- Dart SDK ≥ 3.0
- Android Studio / VS Code with Flutter plugin
- For Linux: `clang`, `cmake`, `ninja-build`, `pkg-config`, `libgtk-3-dev`, `liblzma-dev`

### Make Targets
```bash
make get          # Fetch Dart dependencies
make lint         # Run static analysis (flutter analyze)
make test         # Run unit tests
make icons        # Generate launcher icons
make run-android  # Run on Android device
make run-linux    # Run on Linux
make build-android    # Build debug APK
make build-linux      # Build debug Linux bundle
make release-android  # Build signed release APK
make release-bundle   # Build signed Google Play AAB
make release-linux    # Build release Linux bundle
make clean        # Remove build artifacts
make nuclear      # Full cache cleanup (Gradle, Pub, Build)
make all          # get, lint, test, build-android, build-linux
```

### Key Dependencies
| Package | Purpose |
|---------|---------|
| `provider` | State management |
| `fl_chart` | Charting and data visualisation |
| `flutter_blue_plus` | Bluetooth device discovery |
| `network_info_plus` | Network interface information |
| `sensors_plus` | Hardware sensor streams |
| `battery_plus` | Battery status monitoring |
| `geolocator` | GPS location access |
| `permission_handler` | Runtime permission management |
| `sqflite` / `sqflite_common_ffi` | Local SQLite database |
| `shared_preferences` | First-launch flag persistence |
| `font_awesome_flutter` | Extended icon set |
| `animations` | Material motion transitions |
| `intl` | Date/time formatting |
| `dart_ping` | Network host discovery |
| `wakelock_plus` | Keep screen awake during scans |

## 📂 Project Structure
```
darkworklabs/
├── lib/
│   ├── main.dart                    # App entry point & MultiProvider setup
│   ├── models/                      # Data models (Device)
│   ├── services/                    # Business logic & data services
│   ├── screens/                     # Feature screens
│   └── widgets/                     # Reusable UI components
├── assets/icon/                     # App icon (SVG + PNG)
├── android/                         # Android platform config
├── linux/                           # Linux platform config
├── test/                            # Unit tests
├── docs/                            # Documentation
├── Makefile                         # Build system targets
├── pubspec.yaml                     # Flutter project manifest
└── analysis_options.yaml            # Dart linter configuration
```

## 📖 Documentation
- [User Guide](USER_GUIDE.md) — Comprehensive feature guide
- [Privacy Policy](PRIVACY_POLICY.md) — Data collection and privacy practices

## ⚖️ License

**Copyright (c) 2025-2026 Dark Work Labs & timotheuzi@hotmail.com**  
Proprietary Software. All Rights Reserved.
