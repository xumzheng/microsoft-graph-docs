---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TiIndicator();
requestBody.setAdditionalInformation('additionalInformation-after-update');

requestBody.setConfidence(42);

requestBody.setDescription('description-after-update');


requestConfiguration = TiIndicatorRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.security().tiIndicatorsById('tiIndicator-id').patch(requestBody, requestConfiguration);


```