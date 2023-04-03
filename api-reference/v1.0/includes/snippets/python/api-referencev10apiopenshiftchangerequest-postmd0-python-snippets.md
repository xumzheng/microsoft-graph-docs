---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OpenShiftChangeRequest();
requestBody.setSenderMessage('Can I take this shift?');

requestBody.setOpenShiftId('577b75d2-a927-48c0-a5d1-dc984894e7b8');


request_config = OpenShiftChangeRequestsRequestBuilderPostRequestConfiguration();

headers = [
	'Authorization' => 'Bearer {token}',
];

request_config.headers = headers;


result = awaitclient.teamsById('team-id').schedule().openShiftChangeRequests().post(requestBody, request_config);


```