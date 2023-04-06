---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeleteTiIndicatorsByExternalIdPostRequestBody()
request_body.setValue(['externalId-value1', 'externalId-value2', ])


request_config = DeleteTiIndicatorsByExternalIdRequestBuilderPostRequestConfiguration(
request_config = DeleteTiIndicatorsByExternalIdRequestBuilderPostRequestConfiguration(query_params=)


result = await client.security.tiIndicators.deleteTiIndicatorsByExternalId.post(request_body, headers=)


```