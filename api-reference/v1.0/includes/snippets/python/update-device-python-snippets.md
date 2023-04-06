---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Device()
request_body.setAccountEnabled(false)


request_config = DeviceRequestBuilderPatchRequestConfiguration(
request_config = DeviceRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.devices_by_id('device-id').patch(request_body, headers=)


```