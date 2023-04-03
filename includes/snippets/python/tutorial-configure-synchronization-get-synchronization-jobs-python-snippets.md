---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = JobsRequestBuilderGetRequestConfiguration();

headers = [
	'Authorization' => 'Bearer {Token}',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.servicePrincipalsById('servicePrincipal-id').synchronization().jobs().get(requestConfiguration);


```