---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Shift()
request_body.id = 'SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8'

request_body.userId = 'c5d0c76b-80c4-481c-be50-923cd8d680a1'

request_body.schedulingGroupId = 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0'

sharedShift = ShiftItem()
sharedShift.displayName = 'Day shift'

sharedShift.notes = 'Please do inventory as part of your shift.'

sharedShift.startDateTime = DateTime('2019-03-11T15:00:00Z')

sharedShift.endDateTime = DateTime('2019-03-12T00:00:00Z')

sharedShift.Theme(ScheduleEntityTheme('blue'))

activitiesShiftActivity1 = ShiftActivity()
activitiesShiftActivity1.isPaid = true

activitiesShiftActivity1.startDateTime = DateTime('2019-03-11T15:00:00Z')

activitiesShiftActivity1.endDateTime = DateTime('2019-03-11T15:15:00Z')

activitiesShiftActivity1.code = ''

activitiesShiftActivity1.displayName = 'Lunch'


activitiesArray []= activitiesShiftActivity1;
sharedShift.activities(activitiesArray)



request_body.sharedShift = sharedShift
draftShift = ShiftItem()
draftShift.displayName = 'Day shift'

draftShift.notes = 'Please do inventory as part of your shift.'

draftShift.startDateTime = DateTime('2019-03-11T15:00:00Z')

draftShift.endDateTime = DateTime('2019-03-12T00:00:00Z')

draftShift.Theme(ScheduleEntityTheme('blue'))

activitiesShiftActivity1 = ShiftActivity()
activitiesShiftActivity1.isPaid = true

activitiesShiftActivity1.startDateTime = DateTime('2019-03-11T15:00:00Z')

activitiesShiftActivity1.endDateTime = DateTime('2019-03-11T15:30:00Z')

activitiesShiftActivity1.code = ''

activitiesShiftActivity1.displayName = 'Lunch'


activitiesArray []= activitiesShiftActivity1;
draftShift.activities(activitiesArray)



request_body.draftShift = draftShift


request_configuration = ShiftsRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').schedule.shifts.post(request_body = request_body)


```