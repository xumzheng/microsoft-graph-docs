---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeleteTiIndicatorsPostRequestBody()
request_body.Value(['id-value1', 'id-value2', ])



request_configuration = DeleteTiIndicatorsRequestBuilderPostRequestConfiguration(
)


result = await client.security.tiIndicators.deleteTiIndicators.post(request_body = request_body)


```