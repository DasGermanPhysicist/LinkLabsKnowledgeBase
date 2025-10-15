# Configuration Guide

> [!info] Navigation
> ← Back to [[index|Partner Support Index]]

> [!abstract] Overview
> Step-by-step configuration procedures for setting up AirFinder IoT asset tracking solutions across multiple verticals, from initial account creation to advanced vertical-specific configurations.

## 🚀 Initial Customer Setup Process

### Step 1: Account Creation and Setup

> [!setup] Foundation Setup
> Establish the basic account structure and administrative access for new customers.

#### Create Customer Account
1. **Access Link Labs Manager portal**
   - Navigate to the Link Labs Manager interface
   - Use administrative credentials to access provisioning tools
   
2. **Input customer information and contact details**
   - Complete customer profile with accurate contact information
   - Set up billing and subscription parameters
   - Configure initial user accounts and permissions

3. **Portal Configuration**
   - Customize dashboard layout for specific vertical use cases
   - Set up organizational structure and asset categories
   - Configure notification preferences and alert recipients
   - Establish reporting schedules and formats

> [!tip] Account Setup Best Practices
> - Use consistent naming conventions for assets and locations
> - Set up role-based access from the beginning
> - Configure backup administrators for redundancy

### Step 2: Device Provisioning

#### SuperTag Configuration

> [!device] Device Setup
> Configure SuperTag devices for optimal performance in various operational environments.

**Basic Settings**
```yaml
Device Configuration:
  - Device ID: Use consistent naming convention
  - Location Update Frequency: 5-15 minutes (recommended for most applications)
  - Battery Optimization: Balanced mode for operational periods
  - Cellular Connectivity: Verify carrier compatibility
```

**Vertical-Specific Settings**
```yaml
Vertical Configuration:
  - Geofencing: 10-meter precision boundaries for facilities
  - Tamper Detection: Adjustable sensitivity based on asset type
  - Emergency Alerts: Immediate notification for critical events
  - Chain of Custody: Enable complete audit trail tracking
```

#### BLE Sensor Integration

> [!sensor] Sensor Configuration
> Set up Bluetooth Low Energy sensors for enhanced monitoring capabilities.

**Sensor Pairing Process**
1. **Enable SSF (Sensor Scanning Framework)** on SuperTags
2. **Configure BLE device filters** and MAC addresses
3. **Set up sensor data collection** parameters
4. **Test sensor connectivity** and data flow

**Door Sensor Configuration**
```yaml
Door Sensor Setup:
  Sensor Type: Door/window sensors
  Alert Triggers: 
    - Open/close events
    - Extended open duration (5+ minutes)
  Notification Recipients: Election officials
  Audit Trail: All access events logged
```

> [!warning] Sensor Range Limitations
> BLE sensors must be within 50 feet of SuperTag devices. Plan sensor placement accordingly and test connectivity before deployment.

## 🏢 Vertical Use Case Configurations

### Elections Vertical

> [!ballot] Election Security
> Complete configuration for election security applications including ballot boxes, voting machines, and sensitive materials.

```yaml
Asset Types: Ballot boxes, voting machines, ballot bags, thumb drives
Key Features: Tamper detection, chain of custody, secure access monitoring
Alerts: 
  - Unauthorized access (immediate notification)
  - Extended open duration (5+ minutes)
  - Movement outside designated areas
  - Tamper detection activation
Reporting: 
  - Real-time security dashboard
  - Chain of custody documentation
  - Compliance reports for regulatory requirements
```

### Emergency Services (Ambulances, Fire Departments)

> [!emergency] Emergency Response
> Track emergency vehicles and critical equipment for optimal response times and resource management.

```yaml
Asset Types: Ambulances, fire trucks, medical equipment, rescue gear
Key Features: Real-time location, route optimization, equipment status
Alerts:
  - Vehicle breakdown or maintenance needs
  - Equipment missing from designated locations
  - Extended response times
  - Unauthorized vehicle usage
Reporting:
  - Response time analytics
  - Equipment utilization reports
  - Maintenance scheduling
```

### Transportation & Logistics

> [!truck] Fleet Management
> Monitor trucking fleets, cargo, and logistics operations for efficiency and security.

```yaml
Asset Types: Trucks, trailers, cargo containers, high-value shipments
Key Features: Route tracking, cargo security, delivery confirmation
Alerts:
  - Route deviations
  - Unauthorized stops or delays
  - Cargo tampering or theft
  - Maintenance requirements
Reporting:
  - Delivery performance metrics
  - Route optimization analysis
  - Security incident reports
```

### Vehicle Loss & Theft Prevention

> [!shield] Asset Protection
> Comprehensive vehicle and equipment protection against theft and unauthorized use.

```yaml
Asset Types: Vehicles, construction equipment, valuable machinery
Key Features: Anti-theft monitoring, recovery assistance, usage tracking
Alerts:
  - Unauthorized movement
  - Geofence violations
  - Tampering attempts
  - Extended idle periods
Reporting:
  - Asset utilization reports
  - Security event summaries
  - Recovery success metrics
```

## ⚙️ Feature Configuration Options

### Location Tracking Settings

> [!location] Positioning Configuration
> Optimize location tracking for specific operational environment requirements.

- **Update Frequency**: 1 minute to 24 hours (recommended default: 5 minutes)
- **Accuracy Mode**: High precision (GPS + WiFi + Cellular)
- **Power Management**: Balanced mode for operational periods
- **Geofencing**: Custom boundaries with 10-meter precision

> [!note] Battery Life Considerations
> More frequent location updates reduce battery life. Balance tracking needs with operational duration requirements.

### Alert Configuration

> [!bell] Notification Management
> Set up comprehensive alerting for operational security events.

- **Immediate Alerts**: SMS, email, push notifications
- **Escalation Rules**: Multiple notification levels with time-based escalation
- **Alert Recipients**: Primary and backup contacts for redundancy
- **Quiet Hours**: Configurable for non-operational periods

**Alert Priority Levels**:
- **Critical**: Security breaches, unauthorized access
- **High**: Equipment movement, extended open periods
- **Medium**: Battery warnings, connectivity issues
- **Low**: Routine status updates, maintenance reminders

### Reporting Options

> [!chart] Data and Analytics
> Configure reporting to meet compliance and operational requirements across verticals.

- **Real-time Dashboard**: Live status and alerts for active monitoring
- **Scheduled Reports**: Daily, weekly, monthly summaries
- **Audit Reports**: Complete chain of custody documentation
- **Compliance Reports**: Regulatory requirement adherence

## 🔧 Advanced Configuration

### Custom Integration Setup

> [!api] System Integration
> Connect AirFinder with existing operational management systems across verticals.

**API Configuration**:
- RESTful API endpoints for data exchange
- Authentication and security token management
- Data format and field mapping
- Error handling and retry logic

**Integration Examples**:
- Fleet management system data feeds
- ERP and inventory management connections
- Security system integration
- Reporting platform connections

### Performance Optimization

> [!performance] System Tuning
> Optimize system performance for large-scale deployments across verticals.

**Optimization Areas**:
- **Device Configuration**: Batch configuration for efficiency
- **Network Performance**: Cellular and WiFi optimization
- **Data Processing**: Real-time vs. batch processing decisions
- **Storage Management**: Data retention and archival policies

## 🔗 Related Documentation

> [!tip] Additional Resources
> These documents provide supporting information for configuration tasks.

### Setup Guides
- [[Quick_Start_Guides|Quick Start Guides]] - Rapid deployment procedures
- [[Features_Tools_Training|Training Materials]] - Platform knowledge requirements

### Technical References
- [[../AirFinder User Guide|AirFinder User Guide]] - Comprehensive platform documentation
- [[../SuperTag User Guide|SuperTag User Guide]] - Device configuration details
- [[../SuperTag Behavior Doc v3.3.1|SuperTag Behavior Documentation]] - Technical specifications

### Use Case Examples
- [[../Elections Use Cases/Elections Use Cases - Ballot Box Monitoring and Security|Elections: Ballot Box Monitoring]] - Election security use case
- [[../Elections Use Cases/Elections Use Case - Voting Machine Monitoring|Elections: Voting Machine Monitoring]] - Equipment tracking
- [[../Elections Use Cases/Elections Use Case - Ballot Bag Tracking|Elections: Ballot Bag Tracking]] - Material custody

### Support Resources
- [[Troubleshooting_Guide|Troubleshooting Guide]] - Configuration issue resolution
- [[Issue_Escalation_Plan|Escalation Plan]] - When to seek additional help

---

> [!success] Configuration Checklist
> Before completing customer setup, verify:
> - [ ] All devices are properly configured and communicating
> - [ ] Geofencing boundaries are accurate and tested
> - [ ] Alert notifications are working and reaching correct recipients
> - [ ] Reporting is configured according to customer requirements
> - [ ] Integration with customer systems is functional (if applicable)
> - [ ] Customer training is completed and documented

> [!warning] Security Considerations
> - Always use secure communication channels for configuration
> - Verify user permissions and access levels regularly
> - Document all configuration changes for audit purposes
> - Test security features under realistic conditions

**Document Version**: 2.0  
**Last Updated**: October 15, 2024  
**Part of**: [[index|Link Labs Partner Support Guide]]
