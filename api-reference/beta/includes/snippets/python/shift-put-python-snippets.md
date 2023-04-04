---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Shift();
additionalData = [
'id' => 'SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8', 
'createdDateTime' => '2019-03-14T04:32:51.451Z', 
'lastModifiedDateTime' => '2019-03-14T05:32:51.451Z', 
'userId' => 'c5d0c76b-80c4-481c-be50-923cd8d680a1', 
'schedulingGroupId' => 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0', 
'lastModifiedBy' => request_body = LastModifiedBy();
		request_body.setApplication(null);

		request_body.setDevice(null);

		request_body.setConversation(null);

user = User();
		user.setId('366c0b19-49b1-41b5-a03f-9f3887bd0ed8');

		user.setDisplayName('John Doe');


request_body.setUser($user);

request_body.setLastModifiedBy($lastModifiedBy);

'sharedShift' => request_body = SharedShift();
		request_body.setDisplayName('Day shift');

		request_body.setNotes('Please do inventory as part of your shift.');

		request_body.setStartDateTime('2019-03-11T15:00:00Z');

		request_body.setEndDateTime('2019-03-12T00:00:00Z');

		request_body.setTheme('blue');

activities1 = ();
		activities1.setIsPaid(true);

		activities1.setStartDateTime('2019-03-11T15:00:00Z');

		activities1.setEndDateTime('2019-03-11T15:15:00Z');

		activities1.setCode('');

		activities1.setDisplayName('Lunch');


activitiesArray []= activities1;
request_body.setActivities(activitiesArray);



request_body.setSharedShift($sharedShift);

'draftShift' => request_body = DraftShift();
	request_body.setDisplayName('Day shift');

	request_body.setNotes('Please do inventory as part of your shift.');

	request_body.setStartDateTime('2019-03-11T15:00:00Z');

	request_body.setEndDateTime('2019-03-12T00:00:00Z');

	request_body.setTheme('blue');

activities1 = ();
	activities1.setIsPaid(true);

	activities1.setStartDateTime('2019-03-11T15:00:00Z');

	activities1.setEndDateTime('2019-03-11T15:30:00Z');

	activities1.setCode('');

	activities1.setDisplayName('Lunch');


activitiesArray []= activities1;
request_body.setActivities(activitiesArray);



request_body.setDraftShift($draftShift);

];
request_body.setAdditionalData(additionalData);



request_config = ShiftRequestBuilderPutRequestConfiguration();

headers = [
'Prefer' => 'return=representation',
];

request_config.headers = headers;


await client.teamsById('team-id').schedule().shiftsById('shift-id').put(request_body, request_config);


```