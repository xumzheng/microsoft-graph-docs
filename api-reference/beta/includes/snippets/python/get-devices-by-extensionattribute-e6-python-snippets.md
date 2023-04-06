---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DevicesRequestBuilderGetRequestConfiguration(
request_config = DevicesRequestBuilderGetRequestConfiguration(query_params=query_params = DevicesRequestBuilderGetQueryParameters()
query_params.filter = "extensionAttributes/extensionAttribute1 eq 'BYOD-Device'"
query_params.count = true

)
query_params = DevicesRequestBuilderGetQueryParameters()
query_params.filter = "extensionAttributes/extensionAttribute1 eq 'BYOD-Device'"
query_params.count = true

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.devices.get(request_config, headers=request_config)


```