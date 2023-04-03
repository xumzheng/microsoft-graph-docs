---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CloudPcDeviceImage();
requestBody.set@odatatype('#microsoft.graph.cloudPcDeviceImage');

requestBody.setDisplayName('Display Name value');

requestBody.setOsBuildNumber('OS Build Number value');

requestBody.setOperatingSystem('Operating System value');

requestBody.setVersion('Version value');

requestBody.setSourceImageResourceId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage');



result = awaitclient.deviceManagement().virtualEndpoint().deviceImages().post(requestBody);


```