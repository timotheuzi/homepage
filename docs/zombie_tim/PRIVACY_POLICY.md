# Privacy Policy

**Effective Date:** March 16, 2026

## Introduction

Zombie Tim ("we", "our", "us") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, and safeguard your information when you use our cross-platform application.

## Information We Collect

### 1. Personal Information
We do not collect any personal information that can identify you individually.

### 2. Local App Data
All data is stored locally on your device using SQLite:
- **Personal Assistant Data**: Reminders, tasks, and notes are stored locally to provide assistant functionality.
- **Dictionary Words and Definitions**: Word definitions from public domain sources for offline dictionary functionality.
- **App Preferences**: User preferences and settings stored locally.
- **Conversation History**: Chat history stored locally to provide context and learning.
- **Security Scan Results**: Network and Bluetooth information is scanned locally and not stored or transmitted.
- **System Information**: OS type, version, and system status used for desktop integration features.

### 3. Internet Access
The app requires internet access for:
- **World Information**: Weather data (Open-Meteo), news headlines (Fark, Yahoo News RSS), and time services.
- **Dictionary Expansion**: Downloading word definitions during initial setup or via "Vocabulary Feast" feature.
- **Social Media**: X/Twitter integration when you provide API credentials (optional feature).
- **Vocabulary Learning**: Fetching random words from the internet to expand Tim's vocabulary.
- No personal data, reminders, tasks, or notes are ever transmitted or collected on our servers.

## Data Storage and Security

- **All data (dictionary, reminders, tasks, notes, chat history) is stored locally on your device.**
- We use a local SQLite "Brain Database" to manage this information.
- No personal information is transmitted to external servers.
- Security scans and system information are processed in-memory only and not persisted.
- We implement industry-standard security measures to protect your locally stored data.

## Third-Party Services

### APIs Used
- **Open-Meteo**: Weather data (no API key required)
- **Fark.com & Yahoo News**: News headlines via RSS feeds
- **Random Word API**: Vocabulary expansion
- **Dictionary API**: Word definitions
- **X/Twitter API**: Optional social media integration (only when you provide credentials)

### Analytics & Tracking
- We do not use third-party analytics services.
- We do not share your data with any external parties.
- No advertising or tracking services are integrated.

## Children's Privacy

Our app is suitable for all ages and does not collect any information from children.

## Permissions

### Desktop Platforms (Linux, Windows, macOS)
- **Network Access**: Required for security monitoring (scanning connections, checking Bluetooth, ping tests).
- **System Command Execution**: Optional feature for running system commands (requires user initiation).
- **File System Access**: For scanning files and exporting notes/tasks.

### Mobile Platforms (Android, iOS)
- **Storage Access**: For file scanning features.
- **Network Access**: For internet-based features (weather, news, vocabulary).

All permissions are used solely for the features described and no data is collected or transmitted.

## Changes to This Privacy Policy

We may update our Privacy Policy from time to time. We will notify you of any changes by posting the new Privacy Policy on this page.

## Contact Us

If you have any questions about this Privacy Policy, please contact us at:

Zombie Tim Development Team
Email: privacy@zombietim.app

## Data Retention

- Assistant data (reminders, tasks, notes) and dictionary data are retained as long as the app is installed.
- Security scan results are not stored; they are generated on-demand and displayed in the chat.
- You can clear all data via the **Settings** menu within the app ("Clear Brain").
- You can also delete all stored data by uninstalling the app.

## Your Rights

You have the right to:
- Access your stored data directly within the app's interfaces (Chat, Tasks, Notes screens).
- Request deletion of your data (via Settings or by uninstalling the app).
- Opt out of any data collection (though this may limit app functionality).
- All your data remains on your device and under your control.

## Feature-Specific Privacy Notes

### Security Monitoring
- All security scans are performed locally on your device.
- Network connection information and Bluetooth device lists are not stored or transmitted.
- Scans are read-only and do not modify system state.

### Social Media (X/Twitter)
- API credentials are stored locally on your device.
- Tweet data is fetched in real-time and not stored permanently.
- You can clear credentials at any time through the chat interface.

### World Information
- Weather and news requests are made to third-party APIs.
- No personal information is sent with these requests.
- Location data for weather is obtained via IP geolocation (ip-api.com) and not stored.

### System Integration
- System commands are executed locally on your device.
- System status information is not stored or transmitted.
- File exports are saved to your device's local storage only.

---

By using Zombie Tim, you agree to the terms of this Privacy Policy.