# Dark Work Labs — User Guide 📘

**Package Name:** `com.darkwork.labs`
**Version:** 1.0.0+1

Welcome to the **Dark Work Labs** user guide. This document provides a comprehensive overview of the application's features, how to interpret the data, and how to maximise your security posture using our tools.

## 1. Introduction

Dark Work Labs is a multi-platform security suite providing real-time monitoring of your network, Bluetooth environment, physical hardware sensors, file system, system resources, and radio frequencies to protect you from digital and physical intrusions. It includes AI-driven learning for threat patterns and a refined Material 3 interface with dark and light themes.

## 2. Key Features

### Network Security Scanner
- Discovers all devices on your WiFi and local network
- Identifies open ports and potential vulnerabilities
- Monitors network traffic patterns for anomalies
- Provides detailed device information (IP, MAC, vendor)

### Bluetooth Monitor
- Scans for nearby Bluetooth devices in real-time
- Detects potential tracking devices (AirTags, SmartTags, etc.)
- Monitors Bluetooth signal strength and proximity
- Alerts on unknown or suspicious devices

### Sensor Analysis
- Monitors accelerometer, gyroscope, magnetometer
- Tracks GPS location and movement patterns
- Detects unusual sensor behaviour or tampering
- Visualises sensor data in real-time graphs

### File System Scanner
- Deep scans internal and external storage
- Identifies suspicious files, scripts, and executables
- Detects malware signatures and behavioural patterns
- Quarantines and securely deletes threats

### System Monitor
- Real-time CPU, memory, and disk usage tracking
- Identifies resource-intensive processes
- Monitors system logs for security events
- Provides performance optimisation recommendations

### Radio Frequency Monitor
- Detects unauthorised radio transmissions (requires SDR hardware)
- Scans common frequencies for surveillance devices
- Identifies signal patterns and modulation types
- Alerts on suspicious RF activity

### AI Neural Core
- Machine learning-based threat pattern detection
- Learns your device's normal behaviour
- Identifies anomalies and potential security risks
- Continuously improves detection accuracy

### Intelligence Dashboard
- Centralised view of all security metrics
- Threat confidence scoring and risk assessment
- Historical data analysis and trend identification
- Exportable reports for security analysis

## 3. Getting Started

### Installation

1. Download the APK from the official source
2. Enable "Install from Unknown Sources" in Android settings
3. Install the application
4. Grant required permissions when prompted

### Required Permissions

The app requires the following permissions to function:

- **Location** - For network discovery and Bluetooth scanning
- **Storage** - For file system scanning
- **Bluetooth** - For Bluetooth device monitoring
- **WiFi** - For network security analysis
- **Notifications** - For security alerts
- **Phone** - For device identification

### Initial Setup

1. Launch the app and complete the onboarding wizard
2. Review and accept the privacy policy
3. Configure your security preferences
4. Run your first full system scan
5. Review the intelligence dashboard

## 4. Using the Application

### Dashboard

The main dashboard provides an overview of your device's security status:

- **Header Stats**: Total nodes, network count, Bluetooth count
- **Filter Bar**: Filter devices by type (network, Bluetooth, sensors)
- **Device Cards**: Detailed information for each detected device
- **Quick Actions**: One-tap access to common security tasks

### Navigation

The app uses a bottom navigation bar with five main sections:

1. **STATUS** - Overview dashboard with security metrics
2. **SENSORS** - Hardware sensor monitoring and analysis
3. **SECURITY** - Threat detection and security scanning
4. **SYSTEM** - System resources and process monitoring
5. **MORE** - Additional settings and information

### Device List

The device list screen shows all detected devices on your network and Bluetooth range:

- **Device Name**: Human-readable name or MAC address
- **IP/MAC Address**: Network identifiers
- **Last Seen**: Timestamp of last detection
- **Type Icon**: Visual indicator of device type
- **Risk Level**: Colour-coded security assessment

**Filtering**: Use the filter chips at the top to show only specific device types.

**Device Details**: Tap any device card to view detailed information including open ports, vendor information, and security assessment.

### Network Security Scanner

To perform a network security scan:

1. Navigate to the Security section
2. Tap "START AUTOMATED SCAN"
3. Wait for the scan to complete
4. Review detected devices and vulnerabilities
5. Take action on identified threats

**Scan Types**:
- **Quick Scan**: Basic device discovery (30 seconds)
- **Deep Scan**: Port scanning and vulnerability assessment (2-5 minutes)
- **Continuous Scan**: Real-time monitoring with alerts

### Bluetooth Monitor

The Bluetooth monitor tracks nearby devices:

1. Ensure Bluetooth is enabled on your device
2. Navigate to the Bluetooth section
3. View real-time list of nearby devices
4. Tap devices for detailed information
5. Set up alerts for unknown devices

**AirTag Detection**: The app specifically alerts on potential tracking devices like Apple AirTags, Samsung SmartTags, and similar Bluetooth beacons.

### Sensor Monitor

Monitor your device's physical sensors:

1. Navigate to the Sensors section
2. View real-time sensor data streams
3. Analyse historical sensor patterns
4. Detect unusual movements or orientations
5. Export sensor data for analysis

**Supported Sensors**:
- Accelerometer
- Gyroscope
- Magnetometer
- GPS/Location
- Proximity sensor
- Light sensor
- Barometer
- Step counter

### File System Scanner

Scan your device for security threats:

1. Navigate to the Security section
2. Select "File System Scanner"
3. Choose scan scope (quick, full, custom)
4. Start the scan
5. Review detected threats
6. Quarantine or delete suspicious files

**Scan Options**:
- **Quick Scan**: Check common threat locations (1-2 minutes)
- **Full Scan**: Complete device scan (10-30 minutes)
- **Custom Scan**: Select specific directories

**Threat Actions**:
- **Quarantine**: Move suspicious files to secure location
- **Delete**: Permanently remove confirmed threats
- **Ignore**: Mark files as safe (adds to whitelist)

### System Monitor

Monitor system resources and processes:

1. Navigate to the System section
2. View real-time CPU, memory, and disk usage
3. Identify resource-intensive processes
4. Monitor system logs for security events
5. Take action on suspicious processes

**System Metrics**:
- CPU usage by core and total
- Memory usage (RAM and swap)
- Disk usage and I/O activity
- Network activity
- Battery consumption
- Temperature monitoring

### Radio Frequency Monitor

Detect unauthorised radio transmissions (requires SDR hardware):

1. Connect a compatible SDR device via USB
2. Navigate to the RF Monitor section
3. Select frequency range to scan
4. Start the scan
5. Review detected signals
6. Identify suspicious transmissions

**Supported Frequencies**:
- 100 kHz - 1.7 GHz (depending on SDR hardware)
- Common surveillance frequencies
- Bluetooth and WiFi bands
- Cellular bands
- ISM bands

### Intelligence Dashboard

The AI-powered intelligence dashboard provides:

1. Navigate to the Intelligence section
2. View threat confidence scores
3. Review anomaly detections
4. Analyse historical trends
5. Export security reports

**AI Features**:
- Behavioural pattern learning
- Anomaly detection
- Threat confidence scoring
- Predictive security analysis
- Automated risk assessment

## 5. Security Features

### Real-Time Protection

The app provides continuous monitoring:

- **Network Monitoring**: Real-time device discovery
- **Bluetooth Alerts**: Instant notification of new devices
- **Sensor Anomalies**: Immediate detection of unusual activity
- **File System Watch**: Continuous threat scanning
- **System Watch**: Process and resource monitoring

### Threat Detection

Multiple detection methods:

- **Signature-Based**: Known malware and threat signatures
- **Behavioural**: Unusual activity patterns
- **Heuristic**: Suspicious file characteristics
- **AI/ML**: Machine learning anomaly detection
- **Network Analysis**: Vulnerability and port scanning

### Privacy & Data Security

Your privacy is paramount:

- **Local Only**: All data stored on your device
- **No Cloud**: No data transmitted to external servers
- **Encrypted Storage**: All data encrypted at rest
- **User Control**: You control all data and settings
- **Transparent**: Open about data collection and usage

## 6. Settings & Configuration

### General Settings

Access settings via the MORE section:

- **Theme**: Choose between light, dark, or system theme
- **Notifications**: Configure alert preferences
- **Scan Frequency**: Adjust automatic scan intervals
- **Data Retention**: Set how long to keep historical data
- **Export/Import**: Backup and restore settings

### Security Settings

- **Auto-Scan**: Enable automatic security scans
- **Real-Time Protection**: Toggle continuous monitoring
- **Threat Actions**: Default actions for detected threats
- **Whitelist**: Manage trusted devices and files
- **Alert Sensitivity**: Adjust detection sensitivity

### Advanced Settings

- **SDR Configuration**: Configure radio hardware settings
- **AI Model**: Adjust machine learning sensitivity
- **Network Profiles**: Save custom network configurations
- **Debug Mode**: Enable detailed logging for troubleshooting

## 7. Troubleshooting

### Common Issues

**App won't start**:
- Ensure you have granted all required permissions
- Check that your Android version is compatible (Android 10+)
- Try clearing app cache and data
- Reinstall the application if necessary

**Bluetooth not working**:
- Ensure Bluetooth is enabled on your device
- Check that location services are enabled (required for Bluetooth scanning)
- Restart Bluetooth if devices aren't detected
- Ensure no other app is blocking Bluetooth access

**Network scan not finding devices**:
- Ensure you're connected to the target network
- Check that the network allows device discovery
- Try a deep scan instead of quick scan
- Verify WiFi is enabled and connected

**File scanner errors**:
- Check storage permissions are granted
- Ensure sufficient storage space is available
- Try scanning individual directories instead of full scan
- Some system directories may be inaccessible (normal)

**Radio monitor not detecting signals**:
- Ensure SDR device is properly connected
- Check USB OTG is enabled on your device
- Verify SDR drivers are installed
- Try different frequency ranges

**High resource usage**:
- Reduce scan frequencies in settings
- Close background processes
- Disable real-time monitoring temporarily
- Check for malware causing high resource usage

### Performance Tips

- **Reduce Scan Frequency**: Lower automatic scan intervals
- **Disable Unused Features**: Turn off monitoring for unused sensors
- **Clear Old Data**: Regularly clear historical data
- **Update Regularly**: Keep the app updated for best performance
- **Restart Periodically**: Restart the app daily for optimal performance

## 8. Best Practices

### Security Best Practices

1. **Regular Scans**: Run full system scans weekly
2. **Update Frequently**: Keep the app and device OS updated
3. **Review Alerts**: Don't ignore security notifications
4. **Whitelist Carefully**: Only whitelist devices/files you trust
5. **Monitor Network**: Regularly check network device list
6. **Check Bluetooth**: Review Bluetooth devices periodically
7. **Analyze Sensors**: Monitor for unusual sensor activity
8. **Review Logs**: Check system logs for suspicious activity

### Privacy Best Practices

1. **Review Permissions**: Regularly review app permissions
2. **Clear Data**: Periodically clear historical data
3. **Export Reports**: Save important security reports
4. **Backup Settings**: Export configuration regularly
5. **Stay Informed**: Read privacy policy updates

## 9. Understanding the Data

### Threat Confidence Scores

The app assigns confidence scores to detected threats:

- **0-25%**: Low confidence - Likely false positive
- **26-50%**: Medium confidence - Requires investigation
- **51-75%**: High confidence - Likely a threat
- **76-100%**: Critical - Immediate action required

### Risk Levels

Devices and threats are categorised by risk:

- **Safe (Green)**: No detected threats
- **Low (Blue)**: Minor issues detected
- **Medium (Yellow)**: Potential security concerns
- **High (Orange)**: Significant security risks
- **Critical (Red)**: Immediate security threat

### Device Types

Common device types you'll see:

- **Phone/Mobile**: Smartphones and tablets
- **Computer**: Laptops, desktops, servers
- **IoT**: Smart home devices, cameras, sensors
- **Network**: Routers, switches, access points
- **Bluetooth**: Headphones, speakers, wearables
- **Unknown**: Unidentified devices (investigate these)

## 10. Ownership & Liability

This application is wholly owned and operated by **Dark Work Labs** and **timotheuzi@hotmail.com**. By using this software, you acknowledge and agree to the following:

**Zero Liability**: Dark Work Labs and timotheuzi@hotmail.com shall not be held responsible for:
- Any security breaches or data loss
- False positives or negatives in threat detection
- Device damage or malfunction
- Privacy violations from third-party apps
- Misuse of the application

**User Responsibility**:
- You are responsible for your device's security
- You must comply with all applicable laws
- You should verify threats before taking action
- You control all data and settings

**No Warranty**: This software is provided "as is" without warranty of any kind.

---

*Dark Work Labs — Your Security, Your Responsibility.*
