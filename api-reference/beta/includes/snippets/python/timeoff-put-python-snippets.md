---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TimesOff();
additionalData = [
'userId' => 'c5d0c76b-80c4-481c-be50-923cd8d680a1', 
'sharedTimeOff' => requestBody = SharedTimeOff();
		requestBody.setTimeOffReasonId('TOR_891045ca-b5d2-406b-aa06-a3c8921245d7');

		requestBody.setStartDateTime('2019-03-11T07:00:00Z');

		requestBody.setEndDateTime('2019-03-12T07:00:00Z');

		requestBody.setTheme('white');


requestBody.setSharedTimeOff($sharedTimeOff);

'draftTimeOff' => requestBody = DraftTimeOff();
		requestBody.setTimeOffReasonId('TOR_891045ca-b5d2-406b-aa06-a3c8921245d7');

		requestBody.setStartDateTime('2019-03-11T07:00:00Z');

		requestBody.setEndDateTime('2019-03-12T07:00:00Z');

		requestBody.setTheme('pink');


requestBody.setDraftTimeOff($draftTimeOff);

];
requestBody.setAdditionalData(additionalData);



request_config = TimeOffRequestBuilderPutRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
];

request_config.headers = headers;


await client.teamsById('team-id').schedule().timesOffById('timeOff-id').put(requestBody, request_config);


```