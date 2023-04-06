---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DevicesRequestBuilderGetRequestConfiguration(
request_config = DevicesRequestBuilderGetRequestConfiguration(query_params=query_params = DevicesRequestBuilderGetQueryParameters()
query_params.select = ["id","extensionAttributes"]

)
query_params = DevicesRequestBuilderGetQueryParameters()
query_params.select = ["id","extensionAttributes"]

)


result = await client.devices.get(request_config, headers=request_config)


```