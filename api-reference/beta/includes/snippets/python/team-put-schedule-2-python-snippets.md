---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Schedule()
request_body.enabled = true

request_body.timeZone = 'America/Chicago'

request_body.ProvisionStatus(OperationStatus('completed'))

request_body.provisionStatusCode=null

request_body.openShiftsEnabled = true

request_body.swapShiftsRequestsEnabled = true

request_body.offerShiftRequestsEnabled = true

request_body.timeOffRequestsEnabled = true

request_body.timeClockEnabled = true

timeClockSettings = TimeClockSettings()
timeClockSettingsApprovedLocation = GeoCoordinates()
timeClockSettingsApprovedLocation.altitude = 1024.13

timeClockSettingsApprovedLocation.latitude = 26.13246

timeClockSettingsApprovedLocation.longitude = 24.34616


timeClockSettings.approvedLocation = timeClockSettingsApprovedLocation

request_body.timeClockSettings = timeClockSettings


request_configuration = ScheduleRequestBuilderPutRequestConfiguration(
)


result = await client.teams_by_id('team-id').schedule.put(request_body = request_body)


```