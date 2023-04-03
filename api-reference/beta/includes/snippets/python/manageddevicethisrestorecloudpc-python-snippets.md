---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = RestoreCloudPcPostRequestBody();
requestBody.setCloudPcSnapshotId('A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8');



graphServiceClient.deviceManagement().managedDevicesById('managedDevice-id').restoreCloudPc().post(requestBody);


```