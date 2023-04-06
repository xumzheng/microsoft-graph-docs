---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TiIndicator()
request_body.setDescription('description-updated')


request_config = TiIndicatorRequestBuilderPatchRequestConfiguration(
request_config = TiIndicatorRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.security.tiIndicators_by_id('tiIndicator-id').patch(request_body, headers=)


```