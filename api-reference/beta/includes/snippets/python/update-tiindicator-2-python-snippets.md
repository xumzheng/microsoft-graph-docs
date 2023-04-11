---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TiIndicator()
request_body.additionalInformation = 'additionalInformation-after-update'

request_body.confidence = 42

request_body.description = 'description-after-update'



request_configuration = TiIndicatorRequestBuilderPatchRequestConfiguration(
headers = {
					'Prefer' : "return=representation",
}

)


result = await client.security.tiIndicators_by_id('tiIndicator-id').patch(request_body = request_body, request_configuration = request_configuration)


```