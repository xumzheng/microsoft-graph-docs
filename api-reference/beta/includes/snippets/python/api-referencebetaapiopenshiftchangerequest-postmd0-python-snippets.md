---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = OpenShiftChangeRequest();
requestBody.setSenderMessage('Can I take this shift?');

requestBody.setOpenShiftId('577b75d2-a927-48c0-a5d1-dc984894e7b8');


requestConfiguration = OpenShiftChangeRequestsRequestBuilderPostRequestConfiguration();

headers = [
	'Authorization' => 'Bearer {token}',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.teamsById('team-id').schedule().openShiftChangeRequests().post(requestBody, requestConfiguration);


```