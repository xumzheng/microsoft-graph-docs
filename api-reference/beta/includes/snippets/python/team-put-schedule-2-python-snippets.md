---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Schedule();
request_body.setEnabled(true);

request_body.setTimeZone('America/Chicago');

request_body.setProvisionStatus(OperationStatus('completed'));

request_body.setProvisionStatusCode(null);

request_body.setOpenShiftsEnabled(true);

request_body.setSwapShiftsRequestsEnabled(true);

request_body.setOfferShiftRequestsEnabled(true);

request_body.setTimeOffRequestsEnabled(true);

request_body.setTimeClockEnabled(true);

timeClockSettings = TimeClockSettings();
timeClockSettingsApprovedLocation = GeoCoordinates();
timeClockSettingsApprovedLocation.setAltitude(1024.13);

timeClockSettingsApprovedLocation.setLatitude(26.13246);

timeClockSettingsApprovedLocation.setLongitude(24.34616);


timeClockSettings.setApprovedLocation($timeClockSettingsApprovedLocation);

request_body.setTimeClockSettings($timeClockSettings);


result = await client.teamsById('team-id').schedule().put(request_body);


```