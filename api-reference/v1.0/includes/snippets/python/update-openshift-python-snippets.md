---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OpenShift()
request_body.schedulingGroupId = 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0'

shared_open_shift = OpenShiftItem()
sharedOpenShift.notes = 'Inventory Management'

sharedOpenShift.open_slot_count = 5

sharedOpenShift.displayName = 'Field shift'

sharedOpenShift.startDateTime = DateTime('2018-10-04T00:58:45.340Z')

sharedOpenShift.endDateTime = DateTime('2018-10-04T09:50:45.332Z')

sharedOpenShift.Theme(ScheduleEntityTheme('white'))

activities_shift_activity1 = ShiftActivity()
activitiesShiftActivity1.is_paid = True

activitiesShiftActivity1.startDateTime = DateTime('2018-10-04T00:58:45.340Z')

activitiesShiftActivity1.endDateTime = DateTime('2018-10-04T01:58:45.340Z')

activitiesShiftActivity1.code = ''

activitiesShiftActivity1.displayName = 'Lunch'


activitiesArray []= activitiesShiftActivity1;
sharedOpenShift.activities(activitiesArray)



request_body.shared_open_shift = sharedOpenShift
request_body.draftOpenShift=null




result = await client.teams_by_id('team-id').schedule.openShifts_by_id('openShift-id').patch(request_body = request_body)


```