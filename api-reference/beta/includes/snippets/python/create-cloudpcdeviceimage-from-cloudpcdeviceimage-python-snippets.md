---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcDeviceImage()
request_body.@odatatype = '#microsoft.graph.cloudPcDeviceImage'

request_body.displayName = 'Display Name value'

request_body.osBuildNumber = 'OS Build Number value'

request_body.operatingSystem = 'Operating System value'

request_body.version = 'Version value'

request_body.sourceImageResourceId = '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage'



request_configuration = DeviceImagesRequestBuilderPostRequestConfiguration(
)


result = await client.deviceManagement.virtualEndpoint.deviceImages.post(request_body = request_body)


```