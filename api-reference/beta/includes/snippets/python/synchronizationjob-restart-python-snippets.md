---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = RestartPostRequestBody();
criteria = SynchronizationJobRestartCriteria();
criteria.setResetScope(SynchronizationJobRestartScope('watermark, escrows, quarantinestate'));


requestBody.setCriteria($criteria);

requestConfiguration = RestartRequestBuilderPostRequestConfiguration();

headers = [
	'Authorization' => 'Bearer <token>',
];

requestConfiguration.headers = headers;


graphServiceClient.servicePrincipalsById('servicePrincipal-id').synchronization().jobsById('synchronizationJob-id').restart().post(requestBody, requestConfiguration);


```