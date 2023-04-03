---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Schedule();
requestBody.setEnabled(true);

requestBody.setTimeZone('America/Chicago');

requestBody.setProvisionStatus(OperationStatus('completed'));

requestBody.setProvisionStatusCode(null);

requestBody.setOpenShiftsEnabled(true);

requestBody.setSwapShiftsRequestsEnabled(true);

requestBody.setOfferShiftRequestsEnabled(true);

requestBody.setTimeOffRequestsEnabled(true);

requestBody.setTimeClockEnabled(true);

timeClockSettings = TimeClockSettings();
timeClockSettingsApprovedLocation = GeoCoordinates();
timeClockSettingsApprovedLocation.setAltitude(1024.13);

timeClockSettingsApprovedLocation.setLatitude(26.13246);

timeClockSettingsApprovedLocation.setLongitude(24.34616);


timeClockSettings.setApprovedLocation($timeClockSettingsApprovedLocation);

requestBody.setTimeClockSettings($timeClockSettings);


result = await client.teamsById('team-id').schedule().put(requestBody);


```