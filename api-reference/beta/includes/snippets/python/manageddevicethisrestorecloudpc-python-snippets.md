---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = RestoreCloudPcPostRequestBody();
request_body.setCloudPcSnapshotId('A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8');



await client.deviceManagement().managedDevicesById('managedDevice-id').restoreCloudPc().post(request_body);


```