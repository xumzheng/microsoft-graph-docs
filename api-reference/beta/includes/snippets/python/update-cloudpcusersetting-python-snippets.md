---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CloudPcUserSetting();
requestBody.set@odatatype('#microsoft.graph.cloudPcUserSetting');

requestBody.setDisplayName('Example');

requestBody.setSelfServiceEnabled(true);

restorePointSetting = CloudPcRestorePointSetting();
restorePointSetting.setFrequencyInHours(16);

restorePointSetting.setUserRestoreEnabled(true);


requestBody.setRestorePointSetting($restorePointSetting);
requestBody.setLocalAdminEnabled(false);



result = await client.deviceManagement().virtualEndpoint().userSettingsById('cloudPcUserSetting-id').patch(requestBody);


```