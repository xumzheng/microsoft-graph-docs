---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = OpenShift();
additionalData = [
'schedulingGroupId' => 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0', 
'sharedOpenShift' => request_body = SharedOpenShift();
		request_body.setNotes('Inventory Management');

		request_body.setOpenSlotCount(5);

		request_body.setDisplayName('Field shift');

		request_body.setStartDateTime('2018-10-04T00:58:45.340Z');

		request_body.setEndDateTime('2018-10-04T09:50:45.332Z');

		request_body.setTheme('white');

activities1 = ();
		activities1.setIsPaid(true);

		activities1.setStartDateTime('2018-10-04T00:58:45.340Z');

		activities1.setEndDateTime('2018-10-04T01:58:45.340Z');

		activities1.setCode('');

		activities1.setDisplayName('Lunch');


activitiesArray []= activities1;
request_body.setActivities(activitiesArray);



request_body.setSharedOpenShift($sharedOpenShift);

'draftOpenShift' => 	null,
];
request_body.setAdditionalData(additionalData);




await client.teamsById('team-id').schedule().openShiftsById('openShift-id').put(request_body);


```