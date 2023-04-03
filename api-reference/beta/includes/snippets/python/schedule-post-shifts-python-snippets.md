---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Shift();
requestBody.setId('SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8');

requestBody.setUserId('c5d0c76b-80c4-481c-be50-923cd8d680a1');

requestBody.setSchedulingGroupId('TAG_228940ed-ff84-4e25-b129-1b395cf78be0');

sharedShift = ShiftItem();
sharedShift.setDisplayName('Day shift');

sharedShift.setNotes('Please do inventory as part of your shift.');

sharedShift.setStartDateTime(DateTime('2019-03-11T15:00:00Z'));

sharedShift.setEndDateTime(DateTime('2019-03-12T00:00:00Z'));

sharedShift.setTheme(ScheduleEntityTheme('blue'));

activitiesShiftActivity1 = ShiftActivity();
activitiesShiftActivity1.setIsPaid(true);

activitiesShiftActivity1.setStartDateTime(DateTime('2019-03-11T15:00:00Z'));

activitiesShiftActivity1.setEndDateTime(DateTime('2019-03-11T15:15:00Z'));

activitiesShiftActivity1.setCode('');

activitiesShiftActivity1.setDisplayName('Lunch');


activitiesArray []= activitiesShiftActivity1;
sharedShift.setActivities(activitiesArray);



requestBody.setSharedShift($sharedShift);
draftShift = ShiftItem();
draftShift.setDisplayName('Day shift');

draftShift.setNotes('Please do inventory as part of your shift.');

draftShift.setStartDateTime(DateTime('2019-03-11T15:00:00Z'));

draftShift.setEndDateTime(DateTime('2019-03-12T00:00:00Z'));

draftShift.setTheme(ScheduleEntityTheme('blue'));

activitiesShiftActivity1 = ShiftActivity();
activitiesShiftActivity1.setIsPaid(true);

activitiesShiftActivity1.setStartDateTime(DateTime('2019-03-11T15:00:00Z'));

activitiesShiftActivity1.setEndDateTime(DateTime('2019-03-11T15:30:00Z'));

activitiesShiftActivity1.setCode('');

activitiesShiftActivity1.setDisplayName('Lunch');


activitiesArray []= activitiesShiftActivity1;
draftShift.setActivities(activitiesArray);



requestBody.setDraftShift($draftShift);


requestResult = graphServiceClient.teamsById('team-id').schedule().shifts().post(requestBody);


```