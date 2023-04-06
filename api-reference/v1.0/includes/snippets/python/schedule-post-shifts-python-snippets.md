---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Shift()
request_body.setId('SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8')

request_body.setUserId('c5d0c76b-80c4-481c-be50-923cd8d680a1')

request_body.setSchedulingGroupId('TAG_228940ed-ff84-4e25-b129-1b395cf78be0')

sharedShift = ShiftItem()
sharedShift.setDisplayName('Day shift')

sharedShift.setNotes('Please do inventory as part of your shift.')

sharedShift.setStartDateTime(DateTime('2019-03-11T15:00:00Z'))

sharedShift.setEndDateTime(DateTime('2019-03-12T00:00:00Z'))

sharedShift.setTheme(ScheduleEntityTheme('blue'))

activitiesShiftActivity1 = ShiftActivity()
activitiesShiftActivity1.setIsPaid(true)

activitiesShiftActivity1.setStartDateTime(DateTime('2019-03-11T15:00:00Z'))

activitiesShiftActivity1.setEndDateTime(DateTime('2019-03-11T15:15:00Z'))

activitiesShiftActivity1.setCode('')

activitiesShiftActivity1.setDisplayName('Lunch')


activitiesArray []= activitiesShiftActivity1;
sharedShift.setActivities(activitiesArray)



request_body.setSharedShift($sharedShift)
draftShift = ShiftItem()
draftShift.setDisplayName('Day shift')

draftShift.setNotes('Please do inventory as part of your shift.')

draftShift.setStartDateTime(DateTime('2019-03-11T15:00:00Z'))

draftShift.setEndDateTime(DateTime('2019-03-12T00:00:00Z'))

draftShift.setTheme(ScheduleEntityTheme('blue'))

activitiesShiftActivity1 = ShiftActivity()
activitiesShiftActivity1.setIsPaid(true)

activitiesShiftActivity1.setStartDateTime(DateTime('2019-03-11T15:00:00Z'))

activitiesShiftActivity1.setEndDateTime(DateTime('2019-03-11T15:30:00Z'))

activitiesShiftActivity1.setCode('')

activitiesShiftActivity1.setDisplayName('Lunch')


activitiesArray []= activitiesShiftActivity1;
draftShift.setActivities(activitiesArray)



request_body.setDraftShift($draftShift)

request_config = ShiftsRequestBuilderPostRequestConfiguration(
request_config = ShiftsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').schedule.shifts.post(request_body, headers=)


```