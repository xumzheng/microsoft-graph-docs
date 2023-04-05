---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TiIndicator()
request_body.setAdditionalInformation('additionalInformation-after-update')

request_body.setConfidence(42)

request_body.setDescription('description-after-update')


request_config = TiIndicatorRequestBuilderPatchRequestConfiguration()

headers = [
	'Prefer' => 'return=representation',
]

request_config.headers = headers


result = await client.security.tiIndicatorsById('tiIndicator-id').patch(request_body, request_config)


```