---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OpenShift()
request_body.setSchedulingGroupId('TAG_228940ed-ff84-4e25-b129-1b395cf78be0')

sharedOpenShift = OpenShiftItem()
sharedOpenShift.setNotes('Inventory Management')

sharedOpenShift.setOpenSlotCount(5)

sharedOpenShift.setDisplayName('Field shift')

sharedOpenShift.setStartDateTime(DateTime('2018-10-04T00:58:45.340Z'))

sharedOpenShift.setEndDateTime(DateTime('2018-10-04T09:50:45.332Z'))

sharedOpenShift.setTheme(ScheduleEntityTheme('white'))

activitiesShiftActivity1 = ShiftActivity()
activitiesShiftActivity1.setIsPaid(true)

activitiesShiftActivity1.setStartDateTime(DateTime('2018-10-04T00:58:45.340Z'))

activitiesShiftActivity1.setEndDateTime(DateTime('2018-10-04T01:58:45.340Z'))

activitiesShiftActivity1.setCode('')

activitiesShiftActivity1.setDisplayName('Lunch')


activitiesArray []= activitiesShiftActivity1;
sharedOpenShift.setActivities(activitiesArray)



request_body.setSharedOpenShift($sharedOpenShift)
request_body.setDraftOpenShift(null)


request_config = OpenShiftRequestBuilderPatchRequestConfiguration(
request_config = OpenShiftRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').schedule.openShifts_by_id('openShift-id').patch(request_body, headers=)


```