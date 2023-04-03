---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TiIndicator();
requestBody.setAdditionalInformation('additionalInformation-after-update');

requestBody.setConfidence(42);

requestBody.setDescription('description-after-update');


request_config = TiIndicatorRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
];

request_config.headers = headers;


result = await client.security().tiIndicatorsById('tiIndicator-id').patch(requestBody, request_config);


```