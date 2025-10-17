
> [!bell] Symptom
> Receiving alerts when no event occurred, or not receiving expected alerts for actual events.


#### Troubleshooting Steps


**1. Device Health**
> [!calibrate] SuperTag and BLE Device Health
> Confirm all devices are healthy and are reporting into [[AirFinder Portal]].

Follow [[Issue - SuperTag Not Reporting]] and [[Issue - BLE Sensors Not Detecting]]

**2. Alert Configuration Review**

> [!settings] Alert Settings Analysis
> Examine alert configuration for accuracy and appropriateness.

- **Geofencing**: Verify geofencing boundaries are correct and appropriate. Boundaries should be about 100 to 300 ft wider than actual physical bounaries
- **Recipients**: Confirm notification recipient settings are current.
- **Test Message**: Upon alert setup a test message is sent to the customer. Confirm its receipt


#### Resolution Steps
- **Device Health**: Resolve any device issues first
- **Reconfigure Boundaries**: Adjust geofencing boundaries if too restrictive/permissive
- **Update Contacts**: Test and update notification delivery methods
- **System Issue**: [[Issue_Escalation_Plan|Escalate to Link Labs]] if platform problem
