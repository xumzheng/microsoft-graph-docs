---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DeviceRequestBuilderGetRequestConfiguration()

query_params = DeviceRequestBuilderGetQueryParameters()
query_params.select = ["id","extensionAttributes"]

request_config.queryParameters = query_params


result = await client.devices._by_id('device-id').get(request_config)


```