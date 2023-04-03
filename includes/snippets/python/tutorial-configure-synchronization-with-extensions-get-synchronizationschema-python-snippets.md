---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = SchemaRequestBuilderGetRequestConfiguration();

headers = [
	'Authorization' => 'Bearer {Token}',
];

request_config.headers = headers;


result = awaitclient.servicePrincipalsById('servicePrincipal-id').synchronization().jobsById('synchronizationJob-id').schema().get(request_config);


```