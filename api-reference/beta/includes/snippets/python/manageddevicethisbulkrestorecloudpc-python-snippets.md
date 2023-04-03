---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BulkRestoreCloudPcPostRequestBody();
requestBody.setManagedDeviceIds(['30d0e128-de93-41dc-89ec-33d84bb662a0', '7c82a3e3-9459-44e4-94d9-b92f93bf78dd', ]);

requestBody.setRestorePointDateTime(DateTime('2021-09-23T04:00:00.0000000'));

requestBody.setTimeRange(RestoreTimeRange('before'));



result = awaitclient.deviceManagement().managedDevices().bulkRestoreCloudPc().post(requestBody);


```