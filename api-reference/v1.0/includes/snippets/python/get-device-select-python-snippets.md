---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = DeviceRequestBuilderGetRequestConfiguration(
request_configuration = DeviceRequestBuilderGetRequestConfiguration(query_params=query_params = DeviceRequestBuilderGetQueryParameters()
query_params['select'] = ["id","extensionAttributes"]

)
query_params = DeviceRequestBuilderGetQueryParameters()
query_params['select'] = ["id","extensionAttributes"]

)


result = await client.devices_by_id('device-id').get(request_configuration)


```