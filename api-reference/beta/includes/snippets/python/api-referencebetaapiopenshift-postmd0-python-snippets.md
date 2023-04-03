---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OpenShift();
requestBody.setId('OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8');

requestBody.setSchedulingGroupId('TAG_228940ed-ff84-4e25-b129-1b395cf78be0');

sharedOpenShift = OpenShiftItem();
sharedOpenShift.setNotes('InventoryManagement');

sharedOpenShift.setOpenSlotCount(2);

sharedOpenShift.setDisplayName('Dayshift');

sharedOpenShift.setStartDateTime(DateTime('2018-10-04T00: 58: 45.340Z'));

sharedOpenShift.setEndDateTime(DateTime('2018-10-04T09: 50: 45.332Z'));

sharedOpenShift.setTheme(ScheduleEntityTheme('white'));

activitiesShiftActivity1 = ShiftActivity();
activitiesShiftActivity1.setIsPaid(true);

activitiesShiftActivity1.setStartDateTime(DateTime('2018-10-04T00: 58: 45.340Z'));

activitiesShiftActivity1.setEndDateTime(DateTime('2018-10-04T01: 58: 45.340Z'));

activitiesShiftActivity1.setCode('');

activitiesShiftActivity1.setDisplayName('Lunch');


activitiesArray []= activitiesShiftActivity1;
sharedOpenShift.setActivities(activitiesArray);



requestBody.setSharedOpenShift($sharedOpenShift);
requestBody.setDraftOpenShift(null);

requestBody.setCreatedDateTime(DateTime('2019-03-14T04: 32: 51.451Z'));

requestBody.setLastModifiedDateTime(DateTime('2019-03-14T05: 32: 51.451Z'));

lastModifiedBy = IdentitySet();
LastModifiedBy.setApplication(null);

LastModifiedBy.setDevice(null);

lastModifiedByUser = Identity();
lastModifiedByUser.setId('366c0b19-49b1-41b5-a03f-9f3887bd0ed8');

lastModifiedByUser.setDisplayName('JohnDoe');


lastModifiedBy.setUser($lastModifiedByUser);
additionalData = [
'conversation' => 	null,
];
lastModifiedBy.setAdditionalData(additionalData);



requestBody.setLastModifiedBy($lastModifiedBy);

request_config = OpenShiftsRequestBuilderPostRequestConfiguration();

headers = [
'Authorization' => 'Bearer {token}',
];

request_config.headers = headers;


result = await client.teamsById('team-id').schedule().openShifts().post(requestBody, request_config);


```