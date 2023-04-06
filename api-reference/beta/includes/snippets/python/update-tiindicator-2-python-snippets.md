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


request_config = TiIndicatorRequestBuilderPatchRequestConfiguration(
request_config = TiIndicatorRequestBuilderPatchRequestConfiguration(query_params=)
headers['Prefer'] = "return=representation"


result = await client.security.tiIndicators_by_id('tiIndicator-id').patch(request_body, request_config, headers=request_config)


```