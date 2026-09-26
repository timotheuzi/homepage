# 🧟 Zombie Tim 🧟

**Zombie Tim** is a cross-platform, AI-powered personal assistant with a twist—he's undead! Tim lives in your device and helps you manage your life while satisfying his hunger for knowledge (and brains).

Built with **Flutter**, Zombie Tim runs seamlessly on Android, iOS, Web, Linux, macOS, and Windows.

## ✨ Features

- **🧠 Interactive Chat**: Talk to Tim via a blood-splattered, animated interface. He responds with a unique zombie personality and learns from your conversations.
- **⚡ Fast Learning**: Tim absorbs up to 30 new words per message in a single local transaction — no network calls or artificial delays in the chat path — then quietly fetches real dictionary definitions for the newest words in the background.
- **💾 Real Memory**: Teach him things — *"my name is…"*, *"the capital of France is Paris"*, *"I like pizza"* — and he stores them in his knowledge base. Ask later (even rephrased, or after an app restart) and he'll actually answer, using exact-match lookup plus a ranked keyword search. He can also recall past conversations ("what did I say about X?").
- **📈 Evolving Intelligence**: Tim's language tier climbs monotonically with interactions and vocabulary — the more you chat and teach, the sharper (and more "with it") he gets. He never glitches on a direct question.
- **📅 Proactive Assistant**: Tim can now manage your schedule:
    - **Reminders**: Set time-based alerts — *"remind me to … in 2 hours"* or *"… at 5pm"* (defaults to about an hour). List them with `show reminders`.
    - **Task Management**: Keep a "to-do" list — `add task`, `show tasks`, `overdue tasks`, `complete task [id]`.
    - **Notes**: Capture quick thoughts — `take note`, `show notes`, `find note [query]`.
- **📚 Dynamic Vocabulary**: Tim learns as you go. Use `eat word <word>` to expand his knowledge base, and `vocabulary` / `brain stats` to see his progress.
- **🔍 Brain Scanning**: Tim can forage through your device storage to find information — or perform a **Mass Vocabulary Feast**, devouring **5,000** random words from the web (fetched in parallel) to boost his IQ.
- **🎱 Magic 8-Ball**: Get undead predictions for your most pressing questions.
- **🌍 World Information**: Ask Tim about the weather, latest news, current time, or even stock prices.
- **💻 System Integration**: On desktop platforms, Tim can help with system tasks, run commands, and provide system status reports — plus care & feeding via `system health`, `check updates`, `run diagnostics`, and `update system`.
- **🩺 System Health Dashboard**: The **Settings** screen shows live Brain Stats, storage permissions, and a **System Health** card with a 0–100 health score, disk/memory/CPU usage, uptime, process count and detected issues — with one-tap **Run Vitals Check** and **Install Updates** actions.
- **🔒 Security Monitoring**: Tim can perform security audits via chat commands - check your network connections, scan for suspicious activity, and monitor Bluetooth devices.
- **🩺 Daily Summary**: Ask for a `daily summary` to get an at-a-glance view of your day, or `summarize` to see what Tim remembers of your conversations.

## 🚀 Getting Started

1. **Installation**: Download the latest release for your platform.
2. **First Run**: Tim will initialize his SQLite "Brain Database" on your device.
3. **Usage**: Jump into the **Chat** screen and start by saying "Hello" or type `help` to see every command Tim knows. The Chat header reminds you that `help` is always available. The more you chat and teach him, the faster he learns.

Refer to the [USER_GUIDE.md](./USER_GUIDE.md) for a full list of commands and interaction tips.

## 🛠️ Building & Releasing

Every build target is wrapped in the `Makefile`, so you rarely need to call `flutter` directly.

### Common targets

| Target | Result |
|---|---|
| `make lint` | `flutter analyze .` across the whole project |
| `make test` / `make unit-tests` | the full `flutter test` suite |
| `make build-apk` | `build/app/outputs/flutter-apk/app-release.apk` (signed) |
| `make build-aab` | `build/app/outputs/bundle/release/app-release.aab` (signed, for Google Play) |
| `make zombie-release.zip` | `zombie-release.zip` — signed APK + AAB + signing bundle |
| `make build-web` / `build-linux` / `build-windows` / `build-macos` | platform builds |
| `make build-macos-podman` / `build-ios-podman` | macOS / iOS builds driven from a Linux host |

Run `make help` for the complete, always-current list.

### Release signing

Signing credentials live in `android/key.properties`, which is git-ignored. Copy `android/key.properties.example` to `android/key.properties` and fill in your values:

```properties
storeFile=../../upload-keystore.jks
storePassword=********
keyAlias=upload
keyPassword=********
```

`android/app/build.gradle.kts` loads that file for its `signingConfigs.release` block (`storeFile`, `storePassword`, `keyAlias`, `keyPassword`). If the file is missing, the build falls back to the bundled development keystore so local builds keep working.

To create the keystore (JKS) itself:

```bash
make keystore          # creates upload-keystore.jks only if it is missing
make keystore FORCE=1  # deliberately regenerate it — changes the app signing identity
```

`make zombie-release.zip` builds the signed APK **and** AAB, exports the public certificate, and bundles all four files into a single archive:

| File | Purpose |
|---|---|
| `app-release.apk` | signed APK for direct install / sideloading |
| `app-release.aab` | signed Android App Bundle for Google Play |
| `upload-keystore.jks` | the private signing keystore |
| `zombietim-certificate.pem` | the public certificate (safe to share) |

Every artifact is signed with the same certificate, so the APK, the AAB and the bundled `.pem` all report the identical SHA-256 fingerprint.

> ⚠️ **Security:** `zombie-release.zip` contains a **private signing key**. Never commit it or post it publicly, and back it up somewhere safe — if that key is lost you can no longer publish updates to the same Play Store listing. All keystores (`*.jks`, `*.keystore`, `*.p12`, `*.pfx`, …), certificates and private keys (`*.pem`, `*.key`, `*.crt`, `*.cer`, `*.der`, …), Apple provisioning profiles, `key.properties` files and distributables (`*.apk`, `*.aab`, `*.ipa`) are ignored by `.gitignore`. If one is ever committed, treat it as compromised and rotate it.

## 🔒 Security

Zombie Tim can perform security audits on your system via chat commands. Type `security scan`, `check network`, or `check bluetooth` in the chat interface to get detailed security reports.

### Security Commands
- **`security scan`** or **`check security`**: Full security audit (network, Bluetooth, suspicious activity)
- **`check network`** or **`network status`**: Quick network overview
- **`check bluetooth`** or **`bluetooth status`**: Bluetooth device monitoring

All scans are performed locally on your device. No data is transmitted. See [USER_GUIDE.md](./USER_GUIDE.md) for detailed usage.

## 🔒 Privacy

Your data stays in your grave. All interactions, reminders, tasks, and notes are stored **locally** on your device using an encrypted-ready SQLite database. No personal data is sent to our servers. See [PRIVACY_POLICY.md](./PRIVACY_POLICY.md) for details.

## 🤝 Contributing

Tim's brain is always expanding! If you'd like to contribute to his development, feel free to submit a pull request or report issues.

---

*Zombie Tim: Keeping your life organized, one brain at a time.* 🧟‍♂️🧠