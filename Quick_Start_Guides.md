# Quick Start Guides

> [!info] Navigation
> ← Back to [[index|Partner Support Index]]

> [!abstract] Overview
> Step-by-step quick start procedures for common AirFinder election security deployments. These guides provide rapid deployment capabilities for time-sensitive election scenarios.

## 🚀 Quick Start 1: Setting Up Your First Ballot Box Monitor

> [!ballot] Ballot Box Security Setup
> Complete ballot box monitoring setup in 15 minutes with door sensor integration.

### Prerequisites
> [!checklist] Required Items
> Ensure all necessary components are available before starting.

- AirFinder account access (apps.airfinder.com)
- SuperTag device with door sensor capability
- Ballot box with sensor mounting capability
- Mobile device for testing and validation

### Setup Steps (15 minutes)

#### Step 1: Portal Access (2 minutes)
> [!web] Login and Navigation
> Access the AirFinder portal and navigate to asset management.

1. **Navigate to apps.airfinder.com**
2. **Enter credentials** and access dashboard
3. **Verify account permissions** for asset creation

#### Step 2: Create New Asset (5 minutes)
> [!plus] Asset Creation
> Create and configure the ballot box asset in the system.

1. **Click "Add Asset"** → **Select "Ballot Box"**
2. **Enter asset details**:
   - Asset ID: Use consistent naming convention (e.g., BB-001-Precinct-A)
   - Location: Specific precinct or facility name
   - Description: Include ballot box serial number and capacity
3. **Assign SuperTag device** to asset using device serial number

#### Step 3: Configure Monitoring (5 minutes)
> [!settings] Security Configuration
> Set up comprehensive monitoring and alerting for the ballot box.

1. **Enable door sensor monitoring**
   - Navigate to asset settings → Sensors tab
   - Enable BLE door sensor detection
   - Configure sensor MAC address and pairing

2. **Set alert recipients and notification methods**
   - Add primary election official contact
   - Add backup contact for redundancy
   - Enable SMS and email notifications

3. **Configure geofencing boundary**
   - Set 10-meter radius around ballot box location
   - Enable entry/exit alerts for unauthorized movement
   - Set alert sensitivity to medium for election environment

#### Step 4: Test System (3 minutes)
> [!test] Validation Testing
> Verify all monitoring functions are working correctly.

1. **Open/close ballot box** to trigger door sensor
2. **Verify alerts are received** by designated personnel within 30 seconds
3. **Check real-time status updates** in portal dashboard
4. **Test geofencing** by briefly moving device outside boundary

### Success Criteria
> [!check] Validation Checklist
> Confirm all criteria are met before considering setup complete.

- [ ] Asset appears on dashboard with "Active" status
- [ ] Door sensor events trigger immediate alerts (<30 seconds)
- [ ] Location updates every 5 minutes
- [ ] All designated personnel receive notifications
- [ ] Geofencing alerts work correctly

> [!tip] Troubleshooting Quick Reference
> If issues occur, check [[Troubleshooting_Guide|Troubleshooting Guide]] for common solutions or [[Issue_Escalation_Plan|escalate]] if needed.

---

## 🗳️ Quick Start 2: Tracking Voting Equipment

> [!computer] Equipment Tracking Setup
> Deploy comprehensive voting equipment tracking in 30 minutes for multiple assets.

### Prerequisites
> [!checklist] Required Components
> Gather all necessary items for multi-asset deployment.

- Multiple SuperTag devices (one per equipment item)
- Voting machines or equipment to track
- Facility layout map with designated storage areas
- Asset inventory list with serial numbers

### Setup Steps (30 minutes)

#### Step 1: Bulk Asset Creation (10 minutes)
> [!upload] Efficient Asset Management
> Use bulk import for efficient setup of multiple assets.

1. **Prepare CSV import file** with asset information:
   ```csv
   Asset ID, Asset Type, Serial Number, Location, Description
   VM-001, Voting Machine, VM123456, Precinct-A, ES&S ExpressPoll
   VM-002, Voting Machine, VM123457, Precinct-A, ES&S ExpressPoll
   ```

2. **Import assets via portal**:
   - Navigate to Assets → Import
   - Upload CSV file and validate data
   - Review and confirm asset creation

#### Step 2: Device Assignment (10 minutes)
> [!device] Hardware Configuration
> Attach and configure SuperTag devices for each asset.

1. **Attach SuperTags** to each piece of equipment
   - Use secure mounting method appropriate for equipment
   - Ensure device placement doesn't interfere with operation
   - Document device serial number to asset mapping

2. **Verify device connectivity**
   - Check cellular signal strength (minimum 2 bars)
   - Confirm device registration in portal
   - Test location accuracy and update frequency

#### Step 3: Geofencing Setup (7 minutes)
> [!map] Location Management
> Create zones and movement rules for equipment tracking.

1. **Create zones** for different areas:
   - Storage areas (warehouse, secure facility)
   - Polling locations (precincts, voting centers)
   - Transport routes (if applicable)

2. **Set up movement alerts**:
   - Configure alerts for movement between zones
   - Set up custody transfer notifications
   - Enable unauthorized movement detection

#### Step 4: Reporting Configuration (3 minutes)
> [!chart] Automated Reporting
> Set up automated reporting for compliance and operations.

1. **Enable automated daily status reports**
   - Configure report recipients and schedule
   - Include asset location, status, and alert summary
   - Set up chain of custody documentation

2. **Configure compliance reporting**
   - Set up weekly equipment utilization reports
   - Enable audit trail documentation
   - Configure regulatory compliance reports

### Success Criteria
> [!check] Multi-Asset Validation
> Verify system functionality across all tracked equipment.

- [ ] All assets appear in dashboard with correct status
- [ ] Location tracking active for all devices
- [ ] Geofencing alerts configured and tested
- [ ] Automated reporting scheduled and functional
- [ ] Chain of custody tracking operational

---

## 🚨 Quick Start 3: Emergency Response Setup

> [!emergency] Crisis Response Configuration
> Establish emergency monitoring and response capabilities in 20 minutes.

### Prerequisites
> [!checklist] Emergency Preparedness
> Ensure emergency response infrastructure is ready.

- Established escalation contacts with 24/7 availability
- Emergency notification systems (SMS, email, phone)
- 24/7 monitoring capabilities or service
- Backup communication methods

### Setup Steps (20 minutes)

#### Step 1: Emergency Contacts (5 minutes)
> [!contact] Contact Management
> Set up comprehensive emergency contact system.

1. **Add primary emergency contacts**:
   - Election officials with 24/7 availability
   - Security personnel and law enforcement contacts
   - Technical support contacts for system issues

2. **Configure multiple notification methods**:
   - Primary: SMS for immediate alerts
   - Secondary: Email for detailed information
   - Tertiary: Phone calls for critical escalation

3. **Test emergency notification delivery**:
   - Send test alerts to all contacts
   - Verify delivery within 60 seconds
   - Confirm acknowledgment procedures

#### Step 2: Critical Alert Configuration (10 minutes)
> [!alert] Alert Management
> Configure immediate response for critical security events.

1. **Define critical events**:
   - Unauthorized access to ballot boxes or voting equipment
   - Device tampering or physical security breaches
   - System outages during election periods
   - Geofencing violations in secure areas

2. **Set immediate notification triggers**:
   - Zero-delay alerts for critical events
   - Automatic escalation for unacknowledged alerts
   - Multiple notification attempts with increasing urgency

3. **Enable escalation rules**:
   - 5-minute escalation for unacknowledged critical alerts
   - Automatic notification of backup contacts
   - Integration with external security systems if available

#### Step 3: Monitoring Dashboard (5 minutes)
> [!dashboard] Real-Time Operations
> Set up comprehensive monitoring for emergency response.

1. **Configure real-time monitoring view**:
   - Create emergency operations dashboard
   - Display all critical assets and their status
   - Enable real-time alert notifications

2. **Set up alert prioritization and filtering**:
   - Critical: Security breaches, unauthorized access
   - High: Equipment movement, system issues
   - Medium: Routine alerts, maintenance notifications

3. **Enable mobile access**:
   - Configure mobile dashboard access for field personnel
   - Set up push notifications for mobile devices
   - Test mobile functionality and responsiveness

### Success Criteria
> [!check] Emergency Readiness Validation
> Confirm emergency response system is fully operational.

- [ ] All emergency contacts configured and tested
- [ ] Critical alerts trigger immediate notifications
- [ ] Escalation procedures tested and validated
- [ ] Real-time monitoring dashboard operational
- [ ] Mobile access functional for field personnel

---

## 🔗 Related Documentation

> [!tip] Additional Resources
> These documents provide deeper guidance for complex deployments.

### Detailed Configuration
- [[Configuration_Guide|Configuration Guide]] - Comprehensive setup procedures
- [[Features_Tools_Training|Training Materials]] - Platform knowledge requirements
- [[Implementation_Timeline|Implementation Timeline]] - Full deployment planning

### Support Resources
- [[Troubleshooting_Guide|Troubleshooting Guide]] - Issue resolution procedures
- [[Issue_Escalation_Plan|Escalation Plan]] - When and how to get help
- [[Chain_of_Command_Support_Structure|Support Structure]] - Contact information

### Use Case Examples
- [[../Elections Use Cases/Elections Use Case - Ballot Box Monitoring and Security|Ballot Box Monitoring]] - Detailed use case
- [[../Elections Use Cases/Elections Use Case - Voting Machine Monitoring|Voting Machine Monitoring]] - Equipment tracking
- [[../Elections Use Cases/Elections Use Case - Efficient Election Equipment Tracking|Equipment Tracking]] - Comprehensive tracking

---

> [!success] Quick Start Best Practices
> - **Test Everything**: Always validate functionality before going live
> - **Document Changes**: Keep records of all configuration changes
> - **Train Users**: Ensure all users understand the system before deployment
> - **Have Backup Plans**: Prepare contingency procedures for system issues

> [!warning] Critical Reminders
> - Verify cellular coverage before deployment
> - Test emergency procedures under realistic conditions
> - Ensure backup contacts are available 24/7 during elections
> - Document all device serial numbers and asset assignments

**Document Version**: 2.0  
**Last Updated**: October 14, 2024  
**Part of**: [[index|EasyVote Partner Support Guide]]
