
> [!sensor] Symptom
> BLE tags or sensors not reporting data in [[AirFinder Portal]].

#### Troubleshooting Steps

**1. SuperTag Configuration**
> [!device] SuperTag BLE Setup
> Verify SuperTag is properly configured for BLE sensor scanning.

Using the [[SuperTag Downlink Tool Config Web UI|Downlink Tool]]:
- **[[SuperTag]] Health**: Verify the [[SuperTag]] is sending messages
- **SSF Status**: Verify SSF is enabled
- **Device Filters**: Check BLE device filters are correct
- **Scanning Mode**: Confirm stationary scanning is enabled if device not moving
- **Scan Interval**: Verify appropriate scan interval for use case (scan interval must be multiple of beaconing frequency of tags, e.g. 1 sec beaconing tags require at least 3 sec scanning interval)

**2. Sensor Status**
> [!battery] BLE Sensor Health
> Check the status and functionality of BLE sensors.

- **Battery Tab**: Some tags, e.g. [[E8 tag]]s require a battery tab to be pulled for activation. If the sensor has never been detected, the tab might not have been pulled. 
- **Battery Level**: Check BLE device battery level (replace if low). Use [[AirFinder Portal]] or [[Link Labs Manager - A Client Edge, Devprops and Props UI]]
- **Range**: Verify sensor is within 50 feet of SuperTag
- **Broadcasting**: Confirm sensor is broadcasting (use BLE scanner app, filter for MacID without colons)

#### Resolution Steps
- **Enable SSF**: Enable SSF scanning if disabled via downlink command
- **Replace Battery**: Replace BLE device battery if low
- **Force Scan**: Force SSF scan via SuperTag [[SuperTag Downlink Tool Config Web UI|Downlink Tool]]
- **Hardware Issue**: Work with Link Labs support to replace BLE sensor if defective
