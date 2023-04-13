---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Schedule()
request_body.enabled = True

request_body.timeZone = 'America/Chicago'

request_body.ProvisionStatus(OperationStatus('completed'))

request_body.provisionStatusCode=null

request_body.open_shifts_enabled = True

request_body.swap_shifts_requests_enabled = True

request_body.offer_shift_requests_enabled = True

request_body.time_off_requests_enabled = True

request_body.time_clock_enabled = True

time_clock_settings = TimeClockSettings()
time_clock_settings_approved_location = GeoCoordinates()
timeClockSettingsApprovedLocation.altitude = 1024.13

timeClockSettingsApprovedLocation.latitude = 26.13246

timeClockSettingsApprovedLocation.longitude = 24.34616


timeClockSettings.approved_location = timeClockSettingsApprovedLocation

request_body.time_clock_settings = timeClockSettings



result = await client.teams_by_id('team-id').schedule.put(request_body = request_body)


```