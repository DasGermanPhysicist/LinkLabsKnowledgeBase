# Troubleshooting Guide

> [!info] Navigation
> ← Back to [[index|Partner Support Index]]

> [!abstract] Overview
> Comprehensive troubleshooting procedures for common AirFinder issues, including step-by-step resolution guides and escalation criteria for election security applications.

## 🔧 Common Issues and Solutions

### Issue 1: Device Not Reporting Location

> [!warning] Symptom
> SuperTag shows "offline" status or last location update is significantly outdated.

#### Troubleshooting Steps

**1. Check Device Status**
> [!check] Device Health Assessment
> Verify basic device functionality and power status.

- **Battery Level**: Verify device power and battery level (>20% required)
- **Signal Strength**: Confirm cellular signal strength (minimum 2 bars)
- **Physical Condition**: Check for physical damage or water exposure
- **LED Indicators**: Observe device LED patterns for status information

**2. Network Connectivity**
> [!network] Communication Verification
> Ensure device can communicate with AirFinder platform.

- **Cellular Coverage**: Verify cellular coverage in device location
- **Network Status**: Check for carrier outages or maintenance windows
- **SIM Card**: Test device with known good SIM card if available
- **APN Settings**: Verify Access Point Name configuration for carrier

**3. Configuration Review**
> [!settings] Settings Validation
> Confirm device configuration is appropriate for current use case.

- **Update Frequency**: Confirm location update frequency settings (not too aggressive)
- **Power Mode**: Verify device is not in power-saving mode during critical periods
- **Geofencing**: Check geofencing configuration for conflicts or errors

#### Resolution Steps
- **Battery <20%**: Replace device or recharge if applicable
- **No Cellular Signal**: Relocate device or install signal booster
- **Configuration Issue**: Reset to default settings and reconfigure
- **Hardware Failure**: [[Issue_Escalation_Plan|Escalate to Link Labs]] for replacement

### Issue 2: BLE Sensors Not Detecting

> [!sensor] Symptom
> Door sensors or other BLE devices not reporting data to SuperTag.

#### Troubleshooting Steps

**1. SuperTag Configuration**
> [!device] SuperTag BLE Setup
> Verify SuperTag is properly configured for BLE sensor scanning.

- **SSF Status**: Verify SSF (Sensor Scanning Framework) is enabled
- **Device Filters**: Check BLE device filters and MAC addresses are correct
- **Scanning Mode**: Confirm stationary scanning is enabled if device not moving
- **Scan Interval**: Verify appropriate scan interval for use case

**2. Sensor Status**
> [!battery] BLE Sensor Health
> Check the status and functionality of BLE sensors.

- **Battery Level**: Check BLE device battery level (replace if low)
- **Range**: Verify sensor is within 50 feet of SuperTag
- **Broadcasting**: Confirm sensor is broadcasting (use BLE scanner app)
- **Interference**: Check for BLE interference from other devices

**3. Pairing Verification**
> [!link] Connection Validation
> Ensure proper pairing between SuperTag and BLE sensors.

- **MAC Address**: Verify correct MAC address entry in system
- **Duplicates**: Check for duplicate MAC addresses in system
- **Test Device**: Test with known working BLE device
- **Pairing Process**: Re-pair devices if necessary

#### Resolution Steps
- **Enable SSF**: Enable SSF scanning if disabled via downlink command
- **Replace Battery**: Replace BLE device battery if low
- **Correct MAC**: Update MAC address if incorrect in system
- **Force Scan**: Force SSF scan via SuperTag Downlink Tool
- **Hardware Issue**: Replace BLE sensor if defective

### Issue 3: False Alerts or Missing Alerts

> [!bell] Symptom
> Receiving alerts when no event occurred, or not receiving expected alerts for actual events.

#### Troubleshooting Steps

**1. Alert Configuration Review**
> [!settings] Alert Settings Analysis
> Examine alert configuration for accuracy and appropriateness.

- **Trigger Sensitivity**: Check alert trigger sensitivity settings
- **Geofencing**: Verify geofencing boundaries are correct and appropriate
- **Recipients**: Confirm notification recipient settings are current
- **Timing**: Review alert timing and escalation rules

**2. Sensor Calibration**
> [!calibrate] Sensor Adjustment
> Fine-tune sensor settings to reduce false positives/negatives.

- **Tamper Sensitivity**: Adjust tamper detection sensitivity levels
- **Door Thresholds**: Recalibrate door sensor open/close thresholds
- **Environmental**: Account for environmental factors (temperature, vibration)
- **Manual Testing**: Test alert triggers manually to verify functionality

**3. System Performance**
> [!performance] Platform Analysis
> Check for system-level issues affecting alert delivery.

- **Processing Delays**: Check for system delays or processing backlogs
- **Delivery Methods**: Verify notification delivery methods are working
- **Alert History**: Review alert history for patterns and anomalies
- **Network Issues**: Check for network connectivity problems

#### Resolution Steps
- **Adjust Sensitivity**: Fine-tune sensitivity settings to reduce false positives
- **Reconfigure Boundaries**: Adjust geofencing boundaries if too restrictive/permissive
- **Update Contacts**: Test and update notification delivery methods
- **System Issue**: [[Issue_Escalation_Plan|Escalate to Link Labs]] if platform problem

### Issue 4: Portal Access or Login Problems

> [!lock] Symptom
> Cannot access AirFinder portal or experiencing authentication failures.

#### Troubleshooting Steps

**1. Credential Verification**
> [!user] Account Status Check
> Verify user account status and credentials.

- **Username/Password**: Confirm username and password are correct
- **Account Status**: Check for account lockouts or suspensions
- **Permissions**: Verify account permissions and access levels
- **Expiration**: Check for password or account expiration

**2. Browser and Network**
> [!browser] Technical Environment
> Eliminate browser and network-related access issues.

- **Cache/Cookies**: Clear browser cache and cookies
- **Browser Test**: Try different browser or incognito mode
- **Network**: Check firewall and network restrictions
- **JavaScript**: Ensure JavaScript is enabled in browser

**3. Account Status**
> [!account] Administrative Review
> Verify account and subscription status.

- **Active Status**: Verify account is active and not expired
- **Billing**: Check subscription status and billing current
- **User Permissions**: Confirm user permissions for specific features
- **Multi-Factor**: Check multi-factor authentication if enabled

#### Resolution Steps
- **Reset Password**: Reset password if forgotten or expired
- **Contact Admin**: Contact administrator for account reactivation
- **Browser Update**: Update browser or try alternative access method
- **Account Issue**: [[Issue_Escalation_Plan|Escalate to Link Labs]] for account problems

## 🔍 Advanced Troubleshooting

### Device Communication Issues

> [!signal] Advanced Connectivity Diagnosis
> Deep-dive troubleshooting for complex communication problems.

#### Signal Strength Analysis
1. **Diagnostics**: Use device diagnostics to check cellular signal quality
2. **Dead Zones**: Identify dead zones or interference sources in deployment area
3. **External Antenna**: Consider external antenna or signal booster installation
4. **Carrier Analysis**: Analyze carrier performance in specific locations

#### Network Configuration
1. **APN Settings**: Verify Access Point Name settings for cellular carrier
2. **Carrier Restrictions**: Check for carrier-specific restrictions or limitations
3. **SIM Testing**: Test with different SIM card if available
4. **Roaming**: Verify roaming settings if devices cross carrier boundaries

### Data Accuracy Problems

> [!accuracy] Precision and Reliability Issues
> Address issues with location accuracy and sensor data reliability.

#### Location Accuracy
1. **GPS Satellites**: Check GPS satellite availability and signal quality
2. **WiFi Database**: Verify WiFi access point database updates
3. **Environmental**: Consider environmental factors (buildings, weather, interference)
4. **Calibration**: Perform location calibration in deployment environment

#### Sensor Data Validation
1. **Manual Verification**: Cross-reference sensor data with manual observations
2. **Calibration Drift**: Check sensor calibration and drift over time
3. **Processing Algorithms**: Verify data processing algorithms are appropriate
4. **Environmental Compensation**: Account for environmental factors affecting sensors

## 📋 Troubleshooting Checklist

> [!checklist] Systematic Approach
> Follow this checklist for consistent troubleshooting methodology.

### Before Starting
- [ ] Gather all relevant information about the issue
- [ ] Document symptoms and error messages
- [ ] Identify affected devices, users, or locations
- [ ] Determine business impact and urgency level

### During Troubleshooting
- [ ] Follow systematic approach from basic to advanced
- [ ] Document all steps taken and results obtained
- [ ] Test solutions thoroughly before considering resolved
- [ ] Communicate progress to customer regularly

### Before Escalation
- [ ] Verify all Level 1 troubleshooting steps completed
- [ ] Document all attempted solutions and results
- [ ] Gather system logs and diagnostic information
- [ ] Assess need for escalation based on [[Issue_Escalation_Plan|escalation criteria]]

## 🔗 Related Documentation

> [!tip] Supporting Resources
> These documents provide additional context and procedures for troubleshooting.

### Technical References
- [[../SuperTag User Guide|SuperTag User Guide]] - Device operation and configuration
- [[../SuperTag Behavior Doc v3.3.1|SuperTag Behavior Documentation]] - Technical specifications
- [[../BLE Tag Hubmode Troubleshooting Process|BLE Troubleshooting Process]] - Advanced BLE issues

### Configuration Support
- [[Configuration_Guide|Configuration Guide]] - Proper setup procedures
- [[Features_Tools_Training|Platform Training]] - Understanding system capabilities
- [[Quick_Start_Guides|Quick Start Guides]] - Basic setup verification

### Process Documentation
- [[Issue_Escalation_Plan|Escalation Plan]] - When and how to escalate issues
- [[Chain_of_Command_Support_Structure|Support Structure]] - Roles and responsibilities

---

> [!success] Resolution Best Practices
> - **Document Everything**: Keep detailed records of issues and resolutions
> - **Test Thoroughly**: Verify solutions work under realistic conditions
> - **Follow Up**: Ensure customer satisfaction with resolution
> - **Learn Continuously**: Update procedures based on new issues encountered

> [!warning] When to Escalate
> Don't hesitate to escalate if:
> - Issue affects election security or integrity
> - Multiple customers are affected
> - Resolution requires platform changes
> - Customer satisfaction is at risk

**Document Version**: 2.0  
**Last Updated**: October 14, 2024  
**Part of**: [[index|EasyVote Partner Support Guide]]
