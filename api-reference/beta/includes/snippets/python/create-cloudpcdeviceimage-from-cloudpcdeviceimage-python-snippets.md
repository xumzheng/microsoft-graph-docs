---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CloudPcDeviceImage();
request_body.set@odatatype('#microsoft.graph.cloudPcDeviceImage');

request_body.setDisplayName('Display Name value');

request_body.setOsBuildNumber('OS Build Number value');

request_body.setOperatingSystem('Operating System value');

request_body.setVersion('Version value');

request_body.setSourceImageResourceId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage');



result = await client.deviceManagement().virtualEndpoint().deviceImages().post(request_body);


```