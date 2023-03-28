---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new SchemaRequestBuilderGetRequestConfiguration();

$headers = [
	'Authorization' => 'Bearer {Token}',
];

$requestConfiguration->headers = $headers;


$requestResult = $graphServiceClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->schema()->get($requestConfiguration);


```