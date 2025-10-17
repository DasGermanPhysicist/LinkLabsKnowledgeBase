
> [!warning] Symptom
> SuperTags shows different position on the map than its real position 
> 

#### Troubleshooting Steps

**1. Check Time of Location Information**
> [!check] Check Location Timestamp
> Verify that both the SuperTag location and real device location are both reported for the same time

- Check timestamp of location fix in location history 

**2. Check Location Type in History View**
> [!check] Check Location Type
> Check the location type of the most recent location in the location history. CellID locations commonly have large offsets to the true device location.

**3. For Failed GPS and WiFi Scans**
> [!failure] Check for Cause: Failed GPS or WiFi Scans
> Environmental variables may cause GPS or WiFi scans to fail, resulting in CellID location fixes.

- Use [[Link Labs Manager - A Client Edge, Devprops and Props UI]] to retrieve details about the last location messages 
#### Resolution Steps

- If the timestamp of the location is out of date, ask the user to perform a [[CloudSync]]
- If the issue is caused by CellID fixes:
	- Change the location order. Usually GPS/WiFi/CellID resolves the issue. 
	- Ask Link Labs support to turn off CellID for this customer completely.
