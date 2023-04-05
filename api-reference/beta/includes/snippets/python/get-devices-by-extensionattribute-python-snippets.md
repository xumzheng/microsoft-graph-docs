---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DevicesRequestBuilderGetRequestConfiguration(
query_params = DevicesRequestBuilderGetQueryParameters()
query_params.filter = "extensionAttributes/extensionAttribute1 eq 'BYOD-Device'"
query_params.count = true

headers = [
'ConsistencyLevel' => 'eventual',
]

)


result = await client.devices.get(request_config)


```