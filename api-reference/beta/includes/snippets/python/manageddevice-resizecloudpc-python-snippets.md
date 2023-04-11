---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ResizeCloudPcPostRequestBody()
request_body.targetServicePlanId = '30d0e128-de93-41dc-89ec-33d84bb662a0'



request_configuration = ResizeCloudPcRequestBuilderPostRequestConfiguration(
)


await client.deviceManagement.managedDevices_by_id('managedDevice-id').resizeCloudPc.post(request_body = request_body)


```