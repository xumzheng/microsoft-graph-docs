---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TimeOffReason();
additionalData = [
'displayName' => 'Vacation', 
'iconType' => 'plane', 
'isActive' => true,
];
requestBody.setAdditionalData(additionalData);



request_config = TimeOffReasonRequestBuilderPutRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
];

request_config.headers = headers;


awaitclient.teamsById('team-id').schedule().timeOffReasonsById('timeOffReason-id').put(requestBody, request_config);


```