---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = RestartPostRequestBody();
criteria = SynchronizationJobRestartCriteria();
criteria.setResetScope(SynchronizationJobRestartScope('watermark, escrows, quarantinestate'));


requestBody.setCriteria($criteria);

request_config = RestartRequestBuilderPostRequestConfiguration();

headers = [
	'Authorization' => 'Bearer <token>',
];

request_config.headers = headers;


awaitclient.servicePrincipalsById('servicePrincipal-id').synchronization().jobsById('synchronizationJob-id').restart().post(requestBody, request_config);


```